pipeline {
  agent agent1
  tools {
    maven 'maven'
  }
    stages {
      stage("Build") {
        steps {
          script {
            echo "<--------building the code--------->"
            sh 'mvn clean install'
          }
        }
      }
    }
}
