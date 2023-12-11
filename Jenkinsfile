pipeline {
    agent any 
    tools {
        maven "Mymaven"
    
    }

        stages {
        stage('Clonerepo') { 
            steps {
              
                git "https://github.com/subhashish21/springboot-hello.git"
            }
        }
            
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

