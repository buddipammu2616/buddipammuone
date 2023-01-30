pipeline{
    
    agent any 
    environment {
        PATH = "/opt/maven3.6/bin:$PATH"
    }
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'master', url: 'https://github.com/buddipammu2616/buddipammuone.git'
                }
            }
        }
        stage('build code') {
            steps {
                script {
                    sh " mvn clean install "
                }
            }
        }
          
            
        
        

            
     }
}
