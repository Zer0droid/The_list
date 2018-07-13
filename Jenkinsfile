pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'npm build'
      }
    }
    stage('Build') {
      steps {
        sh 'npm build'
      }
    }
    stage('test') {
      steps {
        sh 'npm test'
      }
    }
  }
}