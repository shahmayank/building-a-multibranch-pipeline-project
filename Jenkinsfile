pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello world!"'
      }
    }

    stage('Test') {
      steps {
        sh 'echo \'Hello Test World\''
      }
    }

    stage('Deliver for development') {
      steps {
        sh 'echo \'Hello Development\''
      }
    }

  }
}