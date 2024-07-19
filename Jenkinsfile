pipeline {
    agent {
        docker {
            image 'node:16-alpine'
            reuseNode true  // Optional: Reuse the node for multiple stages
            args '-v /Users/saipandu/.docker:/root/.docker'  // Mounting volume for TLS certificates
        }
    }
    environment {
        // Define environment variables here
        DOCKER_TLS_VERIFY = '1'  // Example: Enable TLS verification
    }
    stages {
        stage('Test') {
            steps {
                echo "Testing..."
                sh 'node --version'
                // Add more test commands here
            }
        }

        stage('Build') {
            steps {
                echo "Running tests..."  // Placeholder message
                // Add your build/test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying..."  // Placeholder message
                // Add your deployment steps here
            }
        }
    }
}
