pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o my_program nishaan.cpp' // Compile C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './my_program' // Execute compiled program
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment steps if needed
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
