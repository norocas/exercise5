pipeline {
    agent any
    stages {
        stage('Echo main branch') {
            when {
                branch 'development'
            }
            echo 'Hello from main branch'
        }
        stage('Echo feature branch') {
            when {
                branch 'feature_x'
            }
            echo 'Hello from feature branch'
        }
    }
}
