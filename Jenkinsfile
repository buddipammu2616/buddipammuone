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
    def M2_HOME = tool name:"Maven-3.6", type: "maven"
    def mavenCMD = "${M2_HOME}/bin"
    sh "${mavenCMD} clean package"
   }
}
            
        
    }
}
