pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checkout Stage Started'
                sh '''
                pwd
                ls -lrt
                sleep 10
                '''
            }
        }

        stage('Build') {
            steps {
                ec 'Build Stage Started'
                sh '''
                echo "Building Application"
                sleep 10
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Test Stage Started'
                sh '''
                echo "Testing Application"
                sleep 10
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy Stage Started'
                sh '''
                echo "Deploying Application"
                sleep 10
                '''
            }
        }
    }

    post {
        success {
            echo 'Pipeline Executed Successfully'
        }

        failure {
            echo 'Pipeline Failed'
        }
    }
}