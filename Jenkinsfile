pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from GitHub
                git url: 'https://github.com/username/repository.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands here
                // Example: sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
                // Example: sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add your deploy commands here
            }
        }
    }

    post {
        always {
            echo 'Cleaning up...'
            cleanWs()
        }
    }
}
