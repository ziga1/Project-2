pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                sh 'sudo apt update'
                sh 'sudo apt install -y apache2'
                sh 'sudo git clone https://github.com/ziga1/Project-2.git /var/www/html'
            }
        }
    }
}
