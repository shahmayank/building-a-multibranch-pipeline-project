pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello world!"'
        git(url: 'https://github.com/shahmayank/building-a-multibranch-pipeline-project', branch: 'master')
      }
    }

    stage('Test') {
      steps {
        sh 'echo \'Hello Test World\''
        git(url: 'https://github.com/shahmayank/building-a-multibranch-pipeline-project', branch: 'master')
      }
    }

    stage('Deliver for development') {
      steps {
        sh 'echo \'Hello Development\''
        git(url: 'https://github.com/shahmayank/building-a-multibranch-pipeline-project', branch: 'Development')
      }
    }

    stage('Deploy for production') {
      steps {
        echo 'Done Prod Deployment'
      }
    }

  }
  environment {
    CI = 'true'
  }
}