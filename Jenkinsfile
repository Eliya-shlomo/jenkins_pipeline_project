pipeline {
    agent any
    stages {
        stage('Check Node') {
            steps {
                script {
                    echo "This pipeline is running on node: ${env.NODE_NAME}"
                }
            }
        }
    }
}
