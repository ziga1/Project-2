pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '/usr/bin/ansible-playbook playbook.yml --key-file /home/zsila/id_rsa'
      }
    }
  }
}