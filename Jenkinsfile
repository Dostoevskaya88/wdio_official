pipeline {
  
  agent any 
    tools {
      nodejs '19.8.1'
    }
    stages {
    stage('Install dependencies') {
      steps {
        sh 'npm version'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm run getting-started'
      }
    }   
    }
  }
