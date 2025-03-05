pipeline {
    agent any
    stages {
        stage('CodeScan'){
            steps{
                sh 'trivy fs . -o result.html'
                cat 'cat result.html'
                
            }
        }
        stage('dockerImageBuild'){
            steps{
                sh 'docker -v'
            }
        }
        stage('pushImage'){
            steps{
                sh 'docker ps'
            }
        }
    }
}