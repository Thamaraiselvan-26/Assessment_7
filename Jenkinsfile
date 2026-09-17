pipeline {
    agent any
    parameters {
        choice(name: 'ENVIRONMENT', choices: ['dev', 'staging', 'prod'], description: 'Select deployment environment for Online Exam System')
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Thamaraiselvan-26/Assessment_7.git'
            }
        }
        stage('Show Parameter') {
            steps {
                echo "Target Exam Environment: ${params.ENVIRONMENT}"
            }
        }
        stage('Simulate Build/Deploy') {
            steps {
                echo "Deploying Online Examination and Evaluation System to the ${params.ENVIRONMENT} environment..."
            }
        }
    }
}
