pipeline {
  agent any
  stages {
    stage('code checkout') {
      steps {
        git(url: 'https://github.com/SofianeBraneci/curriculum-app', branch: 'dev')
      }
    }

    stage('log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile'
      }
    }

  }
}