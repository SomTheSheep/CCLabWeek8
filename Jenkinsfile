pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES2UG22CS565-1 man.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES2UG22CS565-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application... (Modify this as needed)'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
