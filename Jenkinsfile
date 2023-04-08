pipeline {
  
  agent any 
    tools {
      nodejs '19.8.1'
    }
    stages {
      stage("build") {
        
        steps {
          sh 'npm install'
          sh 'npm test'
        }
      }
    }
  }
