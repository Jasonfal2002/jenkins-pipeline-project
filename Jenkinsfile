pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                echo 'Tool: Maven'
                echo 'Command: mvn clean package'
            }
        }
        
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests...'
                echo 'Tools: JUnit for unit tests, Selenium for integration tests'
                echo 'Command: mvn test'
            }
        }
        
        stage('Code Analysis') {
            steps {
                echo 'Analyzing code quality...'
                echo 'Tool: SonarQube'
                echo 'Checking for bugs, vulnerabilities, and code smells'
            }
        }
        
        stage('Security Scan') {
            steps {
                echo 'Performing security scan...'
                echo 'Tool: OWASP Dependency-Check'
                echo 'Scanning for known vulnerabilities'
            }
        }
        
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging environment...'
                echo 'Tool: AWS CLI'
                echo 'Target: AWS EC2 staging instance'
            }
        }
        
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging...'
                echo 'Tool: Selenium'
                echo 'Verifying application in production-like environment'
            }
        }
        
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production environment...'
                echo 'Tool: AWS CodeDeploy'
                echo 'Target: AWS EC2 production instance'
            }
        }
    }
}
