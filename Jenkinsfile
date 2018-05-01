pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Example') {
      steps {
        echo "Hello ${params.Name}!"
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
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}