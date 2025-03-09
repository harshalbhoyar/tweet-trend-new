pipeline{
    agent{
        node{
            label 'maven'
        }
    }
 environment{
        MAVEN_HOME = '/opt/apache-maven-3.9.9'
        PATH = "$MAVEN_HOME/bin:$PATH"
    }   
    stages{
        stage('build'){
            steps{
                echo "----------- build started ----------"
                sh 'mvn clean deploy'
                echo "----------- build complted ----------"
            }
        }
    }
}