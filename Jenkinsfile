pipeline {
  agent {
    docker {
      image 'python:3.7-slim'
    }

  }
  stages {
    stage('install') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }

    stage('test') {
      steps {
        sh 'python -m pytest tests --cov-report=term --cov=tests/'
      }
    }

  }
}