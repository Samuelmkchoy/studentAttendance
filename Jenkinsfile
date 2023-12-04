pipeline {
    agent any

    tools {
        maven 'Maven' // Use the Maven installation named 'Maven'
    }


        stage('Build') {
            steps {
                script {
                    // Use the 'mvn' command directly
                    sh 'mvn clean install'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Use the 'mvn' command directly
                    sh 'mvn test'
                }
            }
        }
    }
}
