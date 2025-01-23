pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
                echo 'Code checkout completed!'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo "Build process executed."'
            }
        }
    }
    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
