pipeline {
    agent any
    stages {
        stage('Hello World') {
            steps {
                echo 'Hello, World!'
            }
        }
    }
    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
