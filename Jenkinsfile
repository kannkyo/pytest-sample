pipeline {
  agent {
    docker {
      image 'python:3.7-slim'
    }

  }
  stages {
    stage('install') {
      steps {
        sh '''ls -al
# pip install -r requirements.txt'''
      }
    }

    stage('test') {
      steps {
        sh '''ls -al
# python -m pytest tests --cov-report=term --cov=tests/'''
      }
    }

  }
}