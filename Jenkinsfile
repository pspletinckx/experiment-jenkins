pipeline {
  agent {
    docker {
      image 'alpine/git'
    }

  }
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        sh 'git clone https://git.shibboleth.net/git/java-opensaml'
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
  environment {
    Secret = 'mysecret'
  }
}