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
        sh 'sh \'./jenkins/scripts/test.sh\''
      }
    }

  }
}