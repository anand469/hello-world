pipeline {
  agent agent1
  tools {
    maven 'maven'
  }
    stages {
      stage("Build") {
        steps {
          echo "<--------building the code--------->"
          sh 'mvn clean install'
        }
      }
    }
}
