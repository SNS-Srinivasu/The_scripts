pipeline {
    agent any
    tools{
        maven 'maven3'
    }
    stages {
        stage('Clean Workspace'){
            steps {
                cleanWs()
            }
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "build is complete "
            }
        }
        stage('Test') {
            steps {
                echo "test is complete "
            }
        }
        stage('Deploy') {
            steps {
                echo "deploy is complete"
            }
        }
    }
}
