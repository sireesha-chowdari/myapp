pipeline {
    agent any

    environment {
        GIT_CREDENTIALS_ID = 'github-token'  // Must match the ID you set in Jenkins
    }

    stages {
        stage('Clone Repo') {
            steps {
                git(
                    url: 'https://github.com/sireesha-chowdari/myapp.git',  // ✅ Use your actual repo URL
                    credentialsId: "${GIT_CREDENTIALS_ID}",                 // ✅ Use the saved credentials
                    branch: 'main'                                          // ✅ Use the correct branch
                )
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                // Your install steps
            }
        }

        stage('Run App') {
            steps {
                echo 'Running app...'
                // Your run steps
            }
        }
    }
}


