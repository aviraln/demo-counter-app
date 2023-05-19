pipeline{

    agent{ label 'maven-agent' } 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', url: 'https://github.com/aviraln/demo-counter-app.git'
                }
            }
        }
