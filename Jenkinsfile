pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "building "
                Set up JDK (assuming JDK is installed on Jenkins agents)
                tools { jdk 'jdk11' } 
                
                Set up Maven (assuming Maven is installed on Jenkins agents)
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
