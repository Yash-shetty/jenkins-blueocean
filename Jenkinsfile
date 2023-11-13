pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test steps'
          }
        }

        stage('Test-parllal') {
          steps {
            echo 'Testing parallarly'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to prod'
      }
    }

  }
}