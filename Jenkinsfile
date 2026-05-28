pipeline {
agent any

environment {
    APP_NAME = "MyApp"
}

stages {

    stage('Checkout Code') {
        steps {
            git branch: 'main',
            url: 'https://github.comSaranya7431/Jenkinsfile.git'
        }
    }

    stage('Build') {
        steps {
            echo "Building ${APP_NAME}"

            bat 'dir'

            // Example for Maven project
            // bat 'mvn clean install'

            // Example for Gradle project
            // bat 'gradlew build'

            // Example for Node.js project
            // bat 'npm install'
        }
    }

    stage('Test') {
        steps {
            echo "Running Tests"

            // Maven
            // bat 'mvn test'

            // Gradle
            // bat 'gradlew test'

            // Node.js
            // bat 'npm test'
        }
    }

    stage('Deploy') {
        steps {
            echo "Deploying Application"

            // Example deployment command
            bat 'echo Deployment Successful'
        }
    }
}

post {

    success {
        echo 'Pipeline executed successfully!'
    }

    failure {
        echo 'Pipeline failed!'
    }

    always {
        echo 'Pipeline execution completed.'
    }
}

}
