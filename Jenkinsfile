pipeline {
    agent any


    
    tools {
        maven 'maven3.10'
        jdk 'jdk17'
    }
    stages {
        stage('Compile') {
            steps {
              sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
              sh 'mvn test'
            }
        }
        stage('package') {
            steps {
              sh 'mvn package'
            }
        }
    }
}
