pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Example') {
      steps {
        echo "Hello ${MY_NAME}"
      }
    }
    stage('Java') {
      steps {
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Matt'
  }
}