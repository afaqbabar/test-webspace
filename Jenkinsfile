#!/usr/bin/groovy

pipeline {
  agent any
  stages {
    
    stage('Checkout'){
      steps { 
    cleanWs()
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/afaqbabar/test-webspace.git']]])

 }
}


    stage('Build') {
      steps {
        sh 'echo \'Hi from Build Stage\''
        dir ('.') { sh './update.sh' }
        dir ('.') {sh 'cp robots.txt robots1.txt'}
        sh 'hostname'
      }
    }
    
 
   
 
  }
}

//def buildApp() {
//     sh 'ls -la'
//     sh './update.sh'
//}

