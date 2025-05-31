pipeline {
    agent any

    environment {
        GIT_CREDENTIALS_ID = 'github-token' // Use the Jenkins credentials you added
    }

    stages {
        stage('Clone Repo') {
            steps {
                git(
                    url: 'https://github.com/sireesha-chowdari/myapp.git',
                    credentialsId: "${GIT_CREDENTIALS_ID}",
                    branch: 'main' // Change this if your branch is different
                )
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                // Example: sh 'npm install' or your actual setup commands
            }
        }

        stage('Run App') {
            steps {
                echo 'Running app...'
                // Example: sh 'npm start' or your app run command
            }
        }
    }
}



