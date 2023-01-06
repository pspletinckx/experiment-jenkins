pipeline {
  agent any
  stages {
    stage('Clone repo') {
      agent any
      steps {
        git(url: 'git@github.com:pspletinckx/eidas-build-train.git', branch: 'master', credentialsId: 'githubPat')
      }
    }

  }
}