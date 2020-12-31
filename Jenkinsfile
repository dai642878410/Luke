pipeline {
  agent any
  stages {
    stage('prepare') {
      parallel {
        stage('prepare') {
          steps {
            sh 'echo "start to prepare"'
            echo 'Hi everyone'
            sleep 1
          }
        }

        stage('pre2') {
          steps {
            sh 'ls -al'
            sh 'pwd'
          }
        }

        stage('Check') {
          steps {
            sh '''echo "check"

'''
          }
        }

      }
    }

    stage('test') {
      steps {
        sleep 2
      }
    }

  }
  environment {
    parameter1 = 'test1'
    parameter2 = 'test2'
  }
}