pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
      }
    }

    stage('Stage 2') {
      steps {
        timestamps() {
          echo 'Messa'
          echo 'Another meesage'
        }

      }
    }

  }
}