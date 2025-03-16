pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o output hello.cpp' // Compile C++ file
            }
        }
        stage('Test') {
            steps {
                sh './output' // Run compiled program
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
