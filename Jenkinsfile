pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
               pip install -r requirements.txt
        }

        stage('Run Tests') {
            steps {
               pytest
            }
        }
    }
}