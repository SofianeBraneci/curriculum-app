pipeline {
  agent any
  stages {
    stage('code checkout') {
      steps {
        git(url: 'https://github.com/SofianeBraneci/curriculum-app', branch: 'dev')
      }
    }

    stage('list dirs') {
      steps {
        sh 'ls -la'
      }
    }

  }
}