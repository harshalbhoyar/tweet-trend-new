pipeline{
    agent{
        node{
            label 'maven'
        }
    }
    
    stages{
        stage('clone-code'){
            steps{
                git branch: 'main', url: 'https://github.com/harshalbhoyar/tweet-trend-new.git'
            }
        }
    }
}