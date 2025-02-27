pipeline {
    agent any  // Use any available agent for the job

    stages {
        stage('Clean') {
            steps {
                // Run 'mvn clean'
                sh 'mvn clean'
            }
        }
        
        stage('Test') {
            steps {
                // Run 'mvn test'
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                // Run 'mvn package'
                sh 'mvn package'
            }
        }

        stage('Install') {
            steps {
                // Run 'mvn install'
                sh 'mvn install'
            }
        }
    }
    
    post {
        always {
            // Clean up or perform actions after the pipeline runs
            echo 'Pipeline has finished executing.'
        }
    }
}

