#!groovy
pipeline {
  agent {node {label 'build'}}
  
  String buildShell = "${env.buildShell}"
  stages {
    stage('build') {
      steps {
        script{
          mvnHome = tool "maven"
          sh "${mvnHome/bin/mvn ${buildShell}}"
      }
    }
  }
}
