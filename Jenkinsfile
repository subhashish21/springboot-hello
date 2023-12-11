pipeline {
    agent any 
    tools {
        maven 'Mymaven'
    
    }

        stages {
        stage('Clonerepo') { 
            steps {
              
                git "https://github.com/subhashish21/springboot-hello.git"
            }
        }
            
        stage('Compile') { 
            steps{
              
                bat 'mvn  compile'
            }
        }
        stage('testing') { 
            
            steps {
                bat 'mvn test'
            }
        }
    }
}

