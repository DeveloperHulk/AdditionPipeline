pipeline {
    agent any
    
   environment
    {
       PATH = "/opt/maven3/bin:$PATH"
    }
    
    stages {
        stage('Git Checkout') {
            steps {
               git 'https://github.com/DeveloperHulk/AdditionPipeline.git'
            }
        }
         stage("Maven Build")
        {
            steps{
                  sh "mvn clean package"
         }
    }
    }
   
}
