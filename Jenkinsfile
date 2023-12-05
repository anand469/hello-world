pipeline {
    agent agent1

    stages {
        stage('Checkout') {
            steps {
                // Clone the Git repository
                git branch: 'main', credentialsId: 'github_token', url: 'https://github.com/anand469/hello-world.git'
            }
        }

        stage('Build') {
            steps {
                // Your build steps go here
                sh 'echo "Building the project"'
            }
        }

        stage('Test') {
            steps {
                // Your testing steps go here
                sh 'echo "Running tests"'
            }
        }

        stage('Deploy') {
            steps {
                // Your deployment steps go here
                sh 'echo "Deploying the application"'
            }
        }
    }

    post {
        success {
            // Actions to perform when the pipeline succeeds
            echo 'Pipeline succeeded!'

            // You can trigger additional actions or notifications here
        }
        failure {
            // Actions to perform when the pipeline fails
            echo 'Pipeline failed!'

            // You can trigger additional actions or notifications here
        }
    }
}
