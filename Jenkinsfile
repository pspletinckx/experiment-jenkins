pipeline {
  agent any
  stages {
    stage('Clone repo') {
      agent any
      steps {
        git(url: 'https://github.com/pspletinckx/eidas-build-train.git', branch: 'master', credentialsId: 'githubPat2')
        sh 'ls'
      }
    }

    stage('') {
      steps {
        sh 'docker image ls'
      }
    }

  }
}