pipeline {
    agent any
    triggers {
        pollSCM('H/5 * * * *')  // polls every 5 minutes 
    }
    // below are the stages
    stages { 
        stage('Build') {
            steps {
                echo 'Task: Compile the application using a build automation tool.'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests and integration tests.'
                echo 'Tool: JUnit or TestNG'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Task: Analyze code quality and standards.'
                echo 'Tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Task: Perform security scan for vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy application to staging environment.'
                echo 'Tool: AWS EC2, Docker'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests in staging environment.'
                echo 'Tool: Selenium or Postman'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy application to production environment.'
                echo 'Tool: AWS EC2 or Kubernetes'
            }
        }
    }
}
