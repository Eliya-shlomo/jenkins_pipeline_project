pipeline {
    agent any // This tells the master to assign the job to any available agent
    stages {
        stage('Checkout Code') {
            steps {
                echo 'Checking out code...'
                checkout scm // Automatically checks out the repository the pipeline is triggered from
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build command for a Node.js project
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Example deploy script
                sh './deploy.sh'
            }
        }
    }
    post {
        always {
            echo 'Cleaning up workspace...'
            cleanWs() // Cleans up the workspace after the job
        }
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check logs.'
        }
    }
}
