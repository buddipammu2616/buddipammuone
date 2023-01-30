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
        
        stages {
        stage('Build') {
            steps {
                script ('maven'){
                  sh 'mvn version'
                }
            }
            
        
    }
}
