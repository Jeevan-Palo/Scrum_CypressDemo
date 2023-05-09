pipeline {
  agent any
  stages {
    stage('Build and Test') {

      steps {
        // sh 'npm ci'
        // sh "npm run test:ci:record"
        sh 'npm install cypress'
        sh 'npx cypress run'
      }
    }
  }
}