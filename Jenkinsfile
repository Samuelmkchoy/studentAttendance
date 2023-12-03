pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the remote repository
                git 'https://github.com/your-username/your-repository.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    echo 'Hello from Jenkins!'
                    sh 'java -version'
                }
            }
        }

        stage('Test') {
            steps {
                // Run JUnit tests
                sh 'mvn test'
            }
        }
    }
}
