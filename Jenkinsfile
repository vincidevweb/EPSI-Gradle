pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh './gradlew bootJar'
      }
    }
  }
}