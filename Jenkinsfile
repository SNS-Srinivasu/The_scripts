pipeline {
    agent {
    docker { image 'sudo docker pull node:16-alpine' }
  }
    stages {
        stage('test') {
            steps {
                echo "testing..."
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

