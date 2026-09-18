pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Task: Build and package the application code.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit and integration tests.'
                echo 'Tool: JUnit'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse code quality.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: Scan for vulnerabilities.'
                echo 'Tool: OWASP ZAP'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy to staging.'
                echo 'Tool: AWS EC2'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Test the application in staging.'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy to production.'
                echo 'Tool: AWS EC2'
            }
        }
    }
}
