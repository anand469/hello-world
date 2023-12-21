pipeline {
    agent any  // Specify where the pipeline will run

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from version control
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Execute build commands (e.g., Maven, Gradle)
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run automated tests
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy built artifacts to a target environment
                echo 'deploy'
            }
        }
    }
}
