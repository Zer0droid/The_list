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
        emailext(subject: 'APROBAR', body: 'Por favor aprueba', attachLog: true, to: 'tester')
        input 'Arpueba'
      }
    }
  }
}