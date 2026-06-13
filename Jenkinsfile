pipeline {
    agent any

    stages {
        stage('Check Python') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install flask'
            }
        }

        stage('Test Application') {
            steps {
                sh 'python3 -m py_compile app.py'
            }
        }
    }
}
