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

    stage('Clone clone clone') {
      agent any
      steps {
        sh 'git clone https://git.shibboleth.net/git/java-opensaml'
        sh 'git status'
      }
    }

  }
}