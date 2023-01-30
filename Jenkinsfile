pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'master', url: 'https://github.com/buddipammu2616/buddipammuone.git'
                }
            }
        }
        
        stage("Maven clean build") {
  steps { 
    def mavenHome = tool name:"Maven-3.6", type: "maven"
    def mavenCMD = "${mavenHome}/bin/mvn"
    sh "${mavenCMD} clean package"
   }
}
   

            
     }
}
