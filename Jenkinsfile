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
        stage('test') {
            steps {
                echo "Testing..."
                sh 'node --version'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
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
