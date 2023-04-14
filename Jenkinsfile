pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '/usr/bin/ansible-playbook playbook.yml --ask-become-pass'
      }
    }
  }
}
