pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone your GitHub repository
                git 'https://github.com/<your-username>/fullstack-ci-demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install Node.js packages
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                // Run test script from package.json
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                echo 'Build step would go here (e.g., webpack, packaging, etc.)'
            }
        }
    }
}
