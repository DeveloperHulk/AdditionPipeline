pipeline {
    agent any
    
    environment{
        PATH = "/Freshers/Devops/apache-maven-3.6.3/bin:$PATH"
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
