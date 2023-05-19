pipeline{
    agent{label 'maven-agent'}
    stages{
        stage('GIT Checkout'){
            steps{
                git url: 'https://github.com/aviraln/demo-counter-app.git', branch: 'main' 
            }
        }
    }
}
