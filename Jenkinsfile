pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo "Clone started"
                    checkout scm
                }
            }
        }

        stage('Code Build') {
            steps {
                script {
                    echo "Building the code"
                    sh 'mvn install'
                }
            }
        }
    }
}
