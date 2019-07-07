pipeline {
  agent any
  stages {
    stage('Git Clone') {
      steps {
        git 'https://github.com/DavidArenburg/demo-app.git'
      }
    }
    stage('Install') {
      steps {
        sh 'echo npm install'
      }
    }
    stage('TEST') {
      steps {
        sh 'echo npm test'
      }
    }
    stage('BUILD') {
      steps {
        sh 'echo npm run build'
      }
    }
  }
}
