pipeline {
    agent any
    stages {
        stage('CodeScan') {
            steps {
                sh 'trivy fs . -o result.html'
                sh 'uname -r'
                sh 'nproc'
            }
        }
        stage('dockerImageBuild') {
            steps {
                echo 'docker -v'
            }
        }
        stage('pushImage') {
            steps {
                echo 'docker ps'
            }
        }
    }
}