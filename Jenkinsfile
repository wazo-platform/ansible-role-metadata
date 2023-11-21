pipeline {
  agent {
    label 'molecule'
  }
  stages {
    stage ('Test') {
      steps {
        checkout scm
        sh 'tox'
      }
    }
  }
}
