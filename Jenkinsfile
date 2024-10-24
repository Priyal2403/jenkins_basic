pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'npm install'

                // Add build commands, e.g., Maven, Gradle, npm, etc.
                // sh 'mvn clean install' or sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Add test commands, e.g., running unit tests
                // sh 'mvn test' or sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'node app.js'
                // Add deployment commands, e.g., copying files to a server
                // sh 'scp target/*.war user@server:/path/to/deploy'
            }
        }
    }
}
