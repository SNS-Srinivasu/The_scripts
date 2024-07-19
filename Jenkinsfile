pipeline {
    agent {
        docker {
            image 'node:16-alpine'
            reuseNode true
            environment {
                DOCKER_CERT_PATH = '/Users/saipandu/.docker'  // Path to TLS certificates
                DOCKER_TLS_VERIFY = '1'  // Enable TLS verification
            }
        }
    }
    stages {
        stage('Test') {
            steps {
                echo "Testing..."
                sh 'node --version'
                // Add more test commands here as needed
            }
        }

        stage('Build') {
            steps {
                echo "Running tests..."  // Renamed from 'Test' to 'Build' for clarity
                // Add your test execution commands here
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying..."
                // Add your deployment steps here
            }
        }
    }
}
