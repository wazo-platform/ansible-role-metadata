pipeline {
  agent {
    label 'molecule-aws-amd64-debian12-small'
  }
  stages {
    stage ('Test') {
      steps {
        checkout scm
        sh 'tox'
      }
    }
  }
  post {
    always {
      cleanWs()
    }
  }
}
