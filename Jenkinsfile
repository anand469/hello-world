pipeline {
    agent agent1
    stages{
        stage('Checkout'){
            steps{
                script{
                echo "Clone started"
                    gitInfo = checkout scm
               
            }
        }
    }

        stage('code build'){
            stage{
                script{
                    echo "building the code"
                    sh """ mvn install """
                }
            }
        }   
}
}
        
