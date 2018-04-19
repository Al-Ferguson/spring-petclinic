pipeline {
  agent any
  tools {
    maven 'Default'
    jdk 'Default'
  }
  stages {
    stage ('Initialize') {
      steps {
        sh '''
          echo "PATH = ${PATH}"
          echo "HOME = ${HOME}"
        '''
      }
    }
    stage ('Build') {
      sh 'mvn clean package'
    }
  }
}