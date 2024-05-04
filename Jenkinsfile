pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building code using Maven'
                // Add your Maven build commands here
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests'
                // Add your test commands here
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Analyzing code using SonarQube'
                // Add your SonarQube analysis commands here
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing security scan'
                // Add your security scan commands here
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging server'
                // Add your deployment commands here
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging environment'
                // Add your integration test commands here
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production server'
                // Add your deployment commands here
            }
        }
    }
    post {
        success {
            echo 'Pipeline successfully executed!'
            emailtext body: 'Pipeline completed successfully.', subject: 'Pipeline Success', to: 'sofiyan7026@gmail.com'
        }
        failure {
            echo 'Pipeline execution failed!'
            emailtext body: 'Pipeline failed to execute.', subject: 'Pipeline Failure', to: 'sofiyan7026@gmail.com'
        }
    }
}
