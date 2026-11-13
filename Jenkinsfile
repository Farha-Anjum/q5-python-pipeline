pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Syntax Check') {
            steps {
                bat '"C:\\Users\\Miss\\AppData\\Local\\Programs\\Python\\Python37\\python.exe" -m py_compile app.py'
            }
        }

        stage('Run Application') {
            steps {
                bat '"C:\\Users\\Miss\\AppData\\Local\\Programs\\Python\\Python37\\python.exe" app.py'
            }
        }
    }
}