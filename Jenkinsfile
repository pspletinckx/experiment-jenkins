pipeline {
  agent any
  stages {
    stage('Stage1') {
      agent {
        docker {
          image 'alpine/git'
        }

      }
      steps {
        sh 'clone https://git.shibboleth.net/git/java-opensaml'
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