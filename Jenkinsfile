pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git 'https://github.com/kurrasaikumar/spring-petclinic.git'
            }
        }
        
        stage('Clean') {
            steps {
                // Clean the project using Maven
                sh 'mvn clean'
            }
        }

        stage('Test') {
            steps {
                // Run tests using Maven
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                // Package the project using Maven (creates the JAR/WAR file)
                sh 'mvn package'
            }
        }
    }
}
