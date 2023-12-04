pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // Use the correct path to mvn based on your Jenkins configuration
                    sh 'path/to/mvn clean install'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Use the correct path to mvn based on your Jenkins configuration
                    sh 'path/to/mvn test'
                }
            }
        }
    }
}
