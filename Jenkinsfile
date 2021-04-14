#!groovy
  
String buildShell = "${env.buildShell}"

pipeline {
  agent {node {label "build"}}
 
  stages {
    stage("build") {
      steps {
        script{
          mvnHome = tool "maven"
          sh "${mvnHome}/bin/mvn ${buildShell}"
        }
      }
    }
  }
}
