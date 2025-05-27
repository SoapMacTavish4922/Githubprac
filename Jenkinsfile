pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repo...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Replace with actual build commands (e.g., `make`, `npm install`, etc.)
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace with actual test commands
            }
        }
    }
}
