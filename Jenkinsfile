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

    stage('') {
      agent {
        docker {
          image 'alpine/git'
        }

      }
      steps {
        sh 'git clone https://git.shibboleth.net/git/java-opensaml'
      }
    }

  }
}