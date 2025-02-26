pipeline {
    agent { label 'slave-1'}
    
    tools{
        maven 'maven3'
        jdk 'JDK17'
    }

    stages {
        
        stage('compile') {
            steps {
                sh "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
