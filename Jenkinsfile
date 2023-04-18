pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '/usr/bin/ansible-playbook playbook.yml --key-file /var/lib/jenkins/cert/id_rsa'
      }
    }
  }
}