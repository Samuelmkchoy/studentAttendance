pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                script {
                    // Use the 'mvn' command from the configured Maven tool
                    sh 'mvn test'
                }
            }
        }
    }
}
