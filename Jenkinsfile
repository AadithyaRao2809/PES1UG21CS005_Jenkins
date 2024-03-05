pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Move to the 'main' directory
                
                    sh 'g++ main/hello.cpp'
                
            }
        }
        stage('Test') {
            steps {
                // Move to the 'main' directory
                
                    sh './a.out' 
                
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Pending...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
