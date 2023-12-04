pipeline {
    agent any

    stages {
        stage('Print Environment Variables') {
            steps {
                script {
                    sh 'printenv'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh '/path/to/maven test'
                }
            }
        }
    }
}
