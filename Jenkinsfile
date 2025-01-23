pipeline {
    agent any
    stages {
        stage('Hello World') {
            steps {
                echo 'Hello, World! its me eliya!'
            }
        }
    }
    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
