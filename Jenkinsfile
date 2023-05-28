pipeline {
  
  agent any 
    tools {
      nodejs '19.8.1'
    }
    stages {
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        ah 'npm init wdio@latest ./test'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm run deleteCookies'
      }
    }   
    }
  }
