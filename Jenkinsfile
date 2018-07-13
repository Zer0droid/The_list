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
        sh 'npm run test'
        emailext(subject: 'APROBAR', body: 'Por favor aprueba', attachLog: true, to: 'Leon')
        input 'Arpueba'
      }
    }
  }
}