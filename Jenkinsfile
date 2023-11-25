pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/piotrsuchy/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }

  }
}