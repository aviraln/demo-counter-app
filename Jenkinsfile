pipeline{
    agent{label 'maven-agent'}
    stages{
        stage('GIT Checkout'){
            steps{
                git url: 'https://github.com/aviraln/demo-counter-app.git', branch: 'main' 
            }
        }
        stage('Unit Testing'){
            steps{
                sh 'mvn test' 
            }
        }
        stage('Integration Testing'){
            steps{
                sh 'mvn verify -DskipUnitTests' 
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn clean install'
            }
        }
    }
}
