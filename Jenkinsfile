pipeline {
    agent any

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
