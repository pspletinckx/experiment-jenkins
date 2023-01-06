pipeline {
  agent any
  stages {
    stage('Clone repo') {
      agent any
      steps {
        git(url: 'https://<access token>@github.com/pspletinckx/eidas-build-train', branch: 'master', credentialsId: 'githubPat')
      }
    }

  }
}