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
                // Assuming it's a Maven project, build using Maven
                sh 'mvn clean install'
            }
        }
    }
}
