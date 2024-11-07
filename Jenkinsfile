pipeline {
    agent any
    environment {
        GITHUB_TOKEN = credentials('github-token1')  // Reference to the Jenkins credential ID
    }
    stages {
        stage('Checkout') {
            steps {
                // Use HTTPS URL format with the GitHub token for authentication
                git branch: 'main', 
                    credentialsId: 'github-token1', 
                    url: "https://${GITHUB_TOKEN}@github.com/Piyush27933/Jenkins.git"
            }
        }
    }
}

