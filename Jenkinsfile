pipeline {
  agent any

  stages {
    stage('Clone Code') {
      steps {
        git 'https://github.com/Saikanthp/my-app.git'
      }
    }

    stage('Build') {
      steps {
        sh './build.sh'
      }
    }

    stage('Test') {
      steps {
        sh './test.sh'
      }
    }

    stage('Deploy') {
      steps {
        sh './deploy.sh'
      }
    }
  }
}