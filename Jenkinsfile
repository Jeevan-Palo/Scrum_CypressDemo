pipeline {
  agent {
        docker {
            image 'node:16-alpine'
            args '-p 3000:3000'
        }
    }
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
