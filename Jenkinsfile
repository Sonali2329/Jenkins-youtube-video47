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
            echo 'Test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy/print message') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}