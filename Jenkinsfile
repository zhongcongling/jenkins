pipeline {
  agent {
    node {
      label 'build'
    }

  }
  stages {
    stage('shell') {
      steps {
        sh 'ansible --version'
      }
    }

  }
}