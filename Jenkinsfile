pipeline {
    agent { docker { image 'maven:3.9.9-eclipse-temurin-21-alpine' } }

    // tools {
    //     maven 'Maven 3.9.9'
    // }

    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}