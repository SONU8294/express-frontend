pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/sonu8294/express-frontend.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Restart App') {
            steps {
                sh 'pm2 restart express-app || pm2 start "npm start" --name express-app'
            }
        }
    }
}
