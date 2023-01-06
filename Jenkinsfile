pipeline {
  agent any
  stages {
    stage('Clone repo') {
      parallel {
        stage('Clone repo') {
          agent any
          steps {
            git(url: 'https://github.com/pspletinckx/eidas-build-train.git', branch: 'master', credentialsId: 'githubPat2')
            sh 'ls'
          }
        }

        stage('Is docker here then') {
          agent {
            docker {
              image 'docker:dind'
            }

          }
          steps {
            sh 'docker --version'
          }
        }

      }
    }

    stage('is docker here') {
      agent {
        docker {
          image 'docker:dind'
        }

      }
      steps {
        sh 'docker image ls'
      }
    }

  }
}