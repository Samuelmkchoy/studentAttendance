pipeline {
    agent any

    tools {
        gradle 'Gradle' // Use the Gradle installation named 'Gradle'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/your-repository.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    // Run Gradle build
                    sh 'gradle clean build'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Run Gradle tests
                    sh 'gradle test'
                }
            }
        }
    }
}
