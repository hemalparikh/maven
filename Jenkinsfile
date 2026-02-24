pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/hemalparikh/maven.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
