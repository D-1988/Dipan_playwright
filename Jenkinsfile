pipeline {
  agent { 
    any
  }
  stages {
    stage('install playwright') {
      steps {
        
         sh 'npm ci'
      
      }
    }
    stage('help') {
      steps {
        sh 'npx playwright install --with-deps'
      }
    }
    stage('test') {
      steps {
        sh 'npx playwright test'
      }
    }
  }
}
