pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo \'Hi from Build Stage\''
        dir ('.') { sh './update.sh' }
        dir ('.') {sh 'cp robots.txt robots1.txt'}
        sh 'echo \'uptime\''
      }
    }
  }
}

//def buildApp() {
//     sh 'ls -la'
//     sh './update.sh'
//}

