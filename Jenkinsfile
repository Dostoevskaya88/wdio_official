pipeline {
  
  agent any 
    environment {
    CHROME_PATH=‘/opt/google/chrome/google-chrome’
  }
    tools {
      nodejs '19.8.1'
    }
    stages {
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
        sh 'npm run getting-started'
      }
    }   
    }
  }
