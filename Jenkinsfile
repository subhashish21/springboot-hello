pipeline {
    agent any 
    tools {
        maven "3.8.5"
    
    }
    stages {
        stage('Compile and Clean') { 
            steps {
                // Run Maven on a Unix agent.
              
                sh "mvn clean compile"
            }
        }
        stage('testing') { 
            
            steps {
                sh "mvn test"
            }
        }
        stage('package') { 
            steps {
                 mvn "package"
            }
        }
    }
}

