pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '/usr/bin/ansible-playbook playbook.yml --extra-vars "ansible_user=zsila ansible_password=yiga123"'
      }
    }
  }
}
