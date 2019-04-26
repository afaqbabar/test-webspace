pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'Hi from Build Stage\''
        dir ('errors') { sh './update.sh' }
      }
    }
  }
}

//def buildApp() {
//     sh 'ls -la'
//     sh './update.sh'
//}

