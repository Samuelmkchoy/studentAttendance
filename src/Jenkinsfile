pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // Replace '/absolute/path/to/mvn' with the actual path
                    sh '/absolute/path/to/mvn clean install'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Replace '/absolute/path/to/mvn' with the actual path
                    sh '/absolute/path/to/mvn test'
                }
            }
        }
    }
}
