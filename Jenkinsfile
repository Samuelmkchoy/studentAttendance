pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build and Test') {
            steps {
                script {
                    def mvnHome = tool 'MavenInstallationName' // Replace with your configured Maven installation name
                    def mavenCMD = "${mvnHome}/bin/mvn"

                    sh "${mavenCMD} clean test"
                }
            }

            post {
                always {
                    junit '**/target/surefire-reports/*.xml'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded! Yay!'
        }
        failure {
            echo 'Pipeline failed! Oh no!'
        }
    }
}
