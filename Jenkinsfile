pipeline {
  
  agent any 
    tools {nodejs "nodejs"}
    stages {
      stage("build") {
        
        steps {
          sh 'npm install'
          sh 'npm run gettingStarted'
        }
      }
    }
  }
