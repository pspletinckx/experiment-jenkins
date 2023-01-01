pipeline {
  agent any
  stages {
    stage('Pull an image') {
      agent any
      steps {
        sh 'docker pull mongo'
      }
    }

  }
}