pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "building "
                tools { jdk 'jdk11' } 
                tools { maven 'maven3' }  
                sh 'mvn clean package'
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
