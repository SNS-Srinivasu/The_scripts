pipeline {
    agent any
    
    // Define tools outside of stages block
    tools {
        // Define JDK and Maven tools
        jdk 'jdk11'
        maven 'maven3'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh 'mvn clean package'
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

