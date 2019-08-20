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
    stage('mail') {
      steps {
        emailext(subject: 'log ', attachLog: true, body: 'voici les resultat du travail jenkins', from: 'vincent@localhost', to: 'vincidevweb@gmail.com')
      }
    }
  }
}