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
        sh 'npm install'
      }
    }
    stage('TEST') {
      steps {
        sh 'npm test'
      }
    }
    stage('BUILD') {
      steps {
        sh 'npm run build'
      }
    }
    stage('ARTIFACT') {
      steps {
        archiveArtifacts '*.zip'
      }
    }
  }
}