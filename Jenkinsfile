pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Fetching source code from GitHub..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying the application..."
            }
        }

    }

    post {

        success {
            echo "Pipeline executed successfully!"
        }

        failure {
            echo "Pipeline failed. Please check the logs."
        }

        always {
            echo "Pipeline execution finished."
        }

    }
}
