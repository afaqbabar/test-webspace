pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'Hi from Build Stage\''
        buildApp()
      }
    }
  }
}

def buildApp() {
     sh 'ls -la'
}

