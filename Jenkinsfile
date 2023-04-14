pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Build your application here
            }
        }
        stage('Deploy') {
            steps {
                withEnv(['PATH=/usr/local/bin:$PATH']) {
                    sh 'ansible-playbook -i 192.168.8.126, -u zsila playbook.yml'
                }
            }
        }
    }
}
