pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Maven is used for building the project.'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Run JUnit and TestNG tests'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'SonarQube is used for analyzing the code.'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'OWASP Dependency-Check is used for scanning code.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Ansible is used for deploying to staging server.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Selenium is used to run integration tests on staging.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Ansible is used to deploy to production.'
            }
        }
    }
}
