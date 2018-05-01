pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Example') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Java') {
      steps {
        sh 'java -version'
      }
    }
  }
}