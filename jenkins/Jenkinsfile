pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building app..."
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'npm test || true'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t my-app:latest .'
            }
        }
    }
}