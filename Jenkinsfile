pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                git 'https://github.com/AmiraKortam/cloud_task_jen.git'
            }
        }
        stage('Execute Bash Script') {
            steps {
                script {
                    def output = bat(script: 'who.sh', returnStdout: true).trim()
                    echo "Script Output: ${output}"
                }
            }
        }
    }
}
