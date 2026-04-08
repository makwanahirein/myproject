pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '/opt/homebrew/bin/mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh '/opt/homebrew/bin/mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
