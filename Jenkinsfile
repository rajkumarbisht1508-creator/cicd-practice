pipeline {
    agent any
    environment {
        PYTHON = 'C:\\Users\\<you>\\AppData\\Local\\Programs\\Python\\Python310\\python.exe'
    }
    stages {
        stage('Install') {
            steps { bat '"%PYTHON%" -m pip install -r requirements.txt' }
        }
        stage('Unit Tests') {
            steps { bat '"%PYTHON%" -m pytest' }
        }
    }
}