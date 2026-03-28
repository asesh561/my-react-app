pipeline {
    agent {
        docker {
            image 'node:22'
        }
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

       stage('Test') {
    steps {
        echo "No tests configured"
    }
}

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}