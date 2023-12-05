pipeline {
    agent agent1
    tools {
        maven 'maven'
        git 'Default'
    }
    stages {
        stage('Build') {
            steps {
                script {
                    echo "building"
                    sh 'mvn clean install'
                }
            }
        }
    }
}
