pipeline {
    agent agent1
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'maven'
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
