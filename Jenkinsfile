pipeline {
  
  agent any 
    environment {
    CHROME_PATH='/opt/google/chrome/google-chrome'
  }
    tools {
      nodejs '19.8.1'
    }
    stages {
          stage('Build') {
      steps {
        // Set CHROME_PATH before running Chrome-related commands
        withEnv(['CHROME_PATH=' + CHROME_PATH]) {
          sh 'google-chrome --version'
          // Other Chrome-related commands
        }
      }
    }
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
