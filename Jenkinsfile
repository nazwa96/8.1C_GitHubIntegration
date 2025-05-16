pipeline {
    agent any
    stages {
        stage('Build') {
            steps { echo 'Build with Maven or Gradle' }
        }
        stage('Unit & Integration Tests') {
            steps { echo 'Run JUnit + Selenium tests' }
        }
        stage('Code Analysis') {
            steps { echo 'Static code analysis via SonarQube' }
        }
        stage('Security Scan') {
            steps { echo 'Dependency check with OWASP DC' }
        }
        stage('Deploy to Staging') {
            steps { echo 'Deploy Docker image to AWS EC2' }
        }
        stage('Integration Tests on Staging') {
            steps { echo 'API tests with Postman Newman' }
        }
        stage('Deploy to Production') {
            steps { echo 'kubectl apply -f k8s/' }
        }
    }
}
