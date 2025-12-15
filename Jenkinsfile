pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building Docker image...'
                // Локальна збірка Docker-образу
                sh 'docker build -t myapp:latest .' 
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Імітація тестів
                sh 'echo "Tests passed!"' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'Pushing Docker image to DockerHub...' 
            }
        }
    }
}
