pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh './gradlew bootJar'
      }
    }
    stage('test uitaire') {
      steps {
        sh './gradlew test'
      }
    }
    stage('gradelsonar') {
      steps {
        sh './gradlew sonarqube'
      }
    }
  }
}