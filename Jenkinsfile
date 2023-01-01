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

    stage('error') {
      agent {
        docker {
          image 'alpine/git'
        }

      }
      steps {
        git(url: 'git clone https://git.shibboleth.net/git/java-opensaml', branch: 'main')
      }
    }

  }
}