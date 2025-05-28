pipeline {
    agent {
        docker {
            image 'maven:3.9.6-eclipse-temurin-21'
            // args '--network jenkins'
        }
    }

    environment {
        DOCKER_HOST = 'tcp://docker:2375'
    }

    // tools {
    //     maven 'Maven 3.9.9'
    // }

    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}