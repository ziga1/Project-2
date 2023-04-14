pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                sh 'sudo apt update'
                sh 'sudo apt install -y apache2'
                sh 'sudo apt install -y git'
                sh 'sudo git clone https://github.com/ziga1/Project-2.git /var/www/html || true'
                sh 'sudo chmod -R 755 /var/www/html'
                sh 'sudo chown -R www-data:www-data /var/www/html'
            }
        }
    }
}
