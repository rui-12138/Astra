pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '1'
      }
    }

    stage('test') {
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}