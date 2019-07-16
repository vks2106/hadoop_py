pipeline {
    agent { docker { image 'python:latest' }  }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('test') {
            steps {
                sh 'pip install -r requirements.txt'
                sh 'pycodestyle --max-line-length=120 .'
            }
        }
    }
}

