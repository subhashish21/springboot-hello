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
            
        stage('Compile') { 
            steps{
              
                sh "mvn  compile"
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

