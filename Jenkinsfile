pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building code using Maven'
               
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests'
                
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Analyzing code using SonarQube'
               
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing security scan'
                
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging server'
               
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging environment'
                
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production server'
                
            }
        }
    }
    post {
        success {
            echo 'Pipeline successfully executed!'
            mail to: "sofiyan7026@gmail.com",
            subject: "Pipeline Succes",
            body: "It is workings!"    
        }
        failure {
            echo 'Pipeline execution failed!'
            mail to: "sofiyan7026@gmail.com",
            subject: "Pipeline Failurye",
            body: "Check again!"    
        }
    }
}
