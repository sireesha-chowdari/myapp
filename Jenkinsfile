pipeline {
    agent any

    environment {
        GIT_CREDENTIALS_ID = 'github-token'  // <-- Replace with your actual credential ID if different
    }

    stages {
        stage('Clone Repo') {
            steps {
                git(
                    url: 'https://github.com/sireesha-chowdari/myapp.git',
                    credentialsId: "${GIT_CREDENTIALS_ID}",
                    branch: 'main'
                )
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                // Add install commands here
            }
        }

        stage('Run App') {
            steps {
                echo 'Running app...'
                // Add run commands here
            }
        }
    }
}

