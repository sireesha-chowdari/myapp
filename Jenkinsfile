pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'python3 -m venv venv'
                sh './venv/bin/pip install -r requirements.txt'
            }
        }

        stage('Run App') {
            steps {
                echo 'Running Flask App...'
                sh 'nohup ./venv/bin/python3 app.py &'
            }
        }
    }
}
