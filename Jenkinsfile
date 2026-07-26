pipeline {
    agent any
    
    environment {
        PATH = "/opt/homebrew/bin:${env.PATH}"
    }
    
    stages {   
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
