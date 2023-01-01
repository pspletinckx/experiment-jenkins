pipeline {
  agent {
    docker {
      image 'docker:dind'
    }

  }
  stages {
    stage('Pull an image') {
      agent any
      steps {
        sh 'docker pull mongo'
      }
    }

  }
}