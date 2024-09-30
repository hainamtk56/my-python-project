/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    
    stages {
        stage('Install dependencies') {
            steps {
                script {
                    echo 'Installing dependencies...'
                }
            }
        }
        stage('Run Tests') {
            steps {
                script {
                    echo 'Running tests...'
                }
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully!!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
