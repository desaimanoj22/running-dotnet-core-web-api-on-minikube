pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Checkout the source code from your repository
                checkout scm

                // Build your .NET project
                sh 'dotnet build'
            }
        }

        stage('Test') {
            steps {
                // Run tests for your .NET project
                sh 'dotnet test'
            }
        }

        stage('Build Docker Image') {
            steps {
                // Build the Docker image for your .NET project
                sh 'docker build -t your-docker-image-name .'
            }
        }

    }

}
