pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000 -p 5000:5000'
    }

  }
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

    stage('Deploy for production') {
      steps {
        echo 'Done Prod Deployment'
      }
    }

  }
}