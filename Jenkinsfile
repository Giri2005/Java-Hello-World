pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'mvn test'
            }
        }

        stage('Clean') {
            steps {
                echo 'Cleaning...'
                sh 'mvn clean'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished ✅'
        }
    }
}
