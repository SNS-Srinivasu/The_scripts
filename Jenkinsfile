pipeline {
    agent any
    tools{
        jdk 'jdk11'
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
