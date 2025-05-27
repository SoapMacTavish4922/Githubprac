pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning the repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the Java project using Maven...'
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests using Maven...'
                sh 'mvn test'
            }
        }
    }

    post {
        success {
            echo 'Build and tests completed successfully!'
        }
        failure {
            echo 'Build or tests failed.'
        }
    }
}
