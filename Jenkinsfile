pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                // Use the 'tool' step to download and configure Maven
                script {
                    def mvnHome = tool 'Maven'
                    env.PATH = "${mvnHome}/bin:${env.PATH}"
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Now, 'mvn' should be available in the PATH
                    sh 'mvn test'
                }
            }
        }
    }
}
