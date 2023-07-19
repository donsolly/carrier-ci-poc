pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh './gradlew test'
            }
        }
        stage('Deploy to staging') {
            steps {
                echo 'Deploying...'
                sh 'helm upgrade --install --namespace staging my-app ./helm'
            }
        }
    }
}
