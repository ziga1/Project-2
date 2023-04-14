pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                withCredentials([sshUserPrivateKey(credentialsId: '<CREDENTIALS_ID>', keyFileVariable: 'SSH_KEY_FILE', passphraseVariable: 'SSH_PASSPHRASE')]) {
                    sh 'ansible-playbook -i <192.168.8.126>, -u <zsila> playbook.yml'
                }
            }
        }
    }
}
