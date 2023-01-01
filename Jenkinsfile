pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        git(url: 'https://git.shibboleth.net/git/java-opensaml', branch: '4.2.0')
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