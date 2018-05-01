pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Example') {
      steps {
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
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
    TEST_USER = credentials('test-user')
  }
}