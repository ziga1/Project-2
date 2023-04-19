pipeline {
  agent any
  stages {
    stage('Deploy Apache to Remote VM') {
      steps {
        ansiblePlaybook(
          playbook: '${WORKSPACE}/playbook.yml',
          inventory: '${WORKSPACE}/hosts'
        )
      }
    }
  }
}
