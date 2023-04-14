pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                withCredentials([sshUserPrivateKey(credentialsId: '92fe88a0-2a98-4259-a9b1-9cf62b9c5b07', keyFileVariable: 'SSH_KEY_FILE', passphraseVariable: 'SSH_PASSPHRASE')]) {
                    sh 'ansible-playbook -i 192.168.8.126, -u zsila playbook.yml'
                }
            }
        }
    }
}
