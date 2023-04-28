pipeline {
  
  agent any 
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
               stage('Allure test') {
      steps {
     allure includeProperties: false, jdk: '', results: [[path: 'allure-results']]
      }
       }
    }
  }

