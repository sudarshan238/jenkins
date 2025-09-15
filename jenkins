pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository from GitHub
                git branch: 'main', url: 'https://github.com/sudarshan238/jenkins.git'
            }
        }

        stage('Terraform Init') {
            steps {
                // Initialize Terraform
                sh 'terraform init'
            }
        }

        stage('Terraform Plan') {
            steps {
                // Show the Terraform execution plan
                sh 'terraform plan'
            }
        }
    }
}
