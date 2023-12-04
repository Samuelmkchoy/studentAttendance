pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Run test
                    sh 'mvn test'
                }
            }
        }
    }
}
