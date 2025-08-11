pipeline {
  agent {
    label 'molecule-aws'
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
