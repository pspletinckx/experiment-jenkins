pipeline {
  agent any
  stages {
    stage('Clone repo') {
      agent any
      steps {
        git(url: 'https://github.com/pspletinckx/eidas-build-train', branch: 'master', credentialsId: 'githubPat')
      }
    }

  }
}