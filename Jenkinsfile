pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                withCredentials([sshUserPrivateKey(credentialsId: 'a42c468a-a3a9-41bb-8fd1-2673d7744bd5', keyFileVariable: 'SSH_KEY_FILE', passphraseVariable: 'SSH_PASSPHRASE')]) {
                    sh 'ansible-playbook -i 192.168.8.126, -u zsila playbook.yml'
                }
            }
        }
    }
}

