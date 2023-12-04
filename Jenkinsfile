pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Change to the project directory
                    dir('/Users/mingkitchoy/.jenkins/workspace/studentAttendance') {
                        // Run tests
                        sh 'mvn test'
                    }
                }
            }
        }
    }

    post {
        always {
            // Archive test results
            junit '**/target/surefire-reports/*.xml'
        }
    }
}
