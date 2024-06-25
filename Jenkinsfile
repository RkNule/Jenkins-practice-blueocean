pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test par') {
      parallel {
        stage('test ') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy successful'
        sleep 9
      }
    }

  }
}