pipeline {
    agent any
    tools {
        maven 'maver'
    }

    stages {
        stage('Build') {
            steps {
                script {
                    // Run tests
                    sh 'mvn test'
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
