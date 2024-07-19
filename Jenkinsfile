pipeline {
    agent {
        docker {
            image 'node:16-alpine'  // Corrected Docker image name
            reuseNode true          // Reuse the Docker container across multiple stages
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
