pipeline {
  agent any
  environment {
    CHROME_PATH=‘/applications/google-chrome.app/contents/macos/google-chrome’
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
  }
}
