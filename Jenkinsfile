pipeline {
  agent any
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