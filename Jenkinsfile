pipeline {
    agent any

    stages {


        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22AM108-1 main.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './this_file_does_not_exist'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
