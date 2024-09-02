pipeline {
    agent any
    
    stages {
        stage('Clone repository') {
            steps {
                git 'https://github.com/Vedmastaren/my-python-jenkins-pipeline.git'
            }
        }
        
        stage('Install dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run tests') {
            steps {
                sh 'pytest test_app.py'
            }
        }
    }
}
