pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test par') {
          steps {
            echo 'test para'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 10
      }
    }

  }
}