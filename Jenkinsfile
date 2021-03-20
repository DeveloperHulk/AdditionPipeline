pipeline {
    agent any
    
    tools
    {
        maven "maven3"
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
