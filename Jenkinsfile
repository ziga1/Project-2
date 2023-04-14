pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh 'ssh-keyscan 192.168.8.126 >> ~/.ssh/known_hosts'
        sh '/usr/bin/ansible-playbook playbook.yml'
      }
    }
  }
}
