pipeline {
    agent any

    tools {
            maven 'Maven' // Use the Maven installation named 'Maven'
        }
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the remote repository
                git 'https://github.com/Samuelmkchoy/studentAttendance'
            }
        }

        stage('Build') {
            steps {
                script {
                    echo 'Hello from Jenkins!'
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
