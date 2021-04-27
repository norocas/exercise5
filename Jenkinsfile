pipeline {
    agent {
        node {
            label 'master'
        }
    }
    stages {
        stage('Echo main branch') {
            when {
                branch 'development'
            }
            steps{
                sh """
                    echo 'Hello from main branch'
                """
            }
        }
        stage('Echo feature branch') {
            when {
                branch 'feature_x'
            }
            steps{
                sh """
                    echo 'Hello from feature branch'
                """
            }
        }
    }
}
