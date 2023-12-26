pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AmiraKortam/cloud_task_jen.git'
            }
        }
        stage('Execute Bash Script') {
            steps {
                script {
                    bat'who.bat'
                }
            }
        }
    }
}
