/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    
    stages {
        stage('Install dependencies') {
            steps {
                script {
                    echo 'Installing dependencies...'
                    sh 'pip install -r requirements.txt'
                }
            }
        }
        stage('Run Tests') {
            steps {
                script {
                    echo 'Running tests...'
                    sh 'python -m unittest discover -s tests'
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
