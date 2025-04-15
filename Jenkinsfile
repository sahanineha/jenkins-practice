pipeline{
    agent any
    tools {
        maven 'Maven'
    }
    stages{
        stage('download git project'){
            steps{
                git branch: 'master', url: 'https://github.com/jabedhasan21/java-hello-world-with-maven'
            }
        }
        stage('build project'){
            steps{
                sh '''
                    cd $WORKSPACE
                    mvn clean install
                '''
            }
        }
    }
}
