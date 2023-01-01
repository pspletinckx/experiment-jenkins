pipeline {
  agent any
  stages {
    stage('Stage1') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        echo 'Hello'
        sh 'echo "hello"'
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