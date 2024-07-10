pipeline {
    agent any

    stages {
        stage('Git checkout') {
            steps {
                git changelog: false, poll: false, url: 'https://github.com/neerajddun/demo-counter-app.git'
            }
        }
        stage('Unit Test') {
            steps {
                sh 'mvn test' // Changed 'mvn Test' to 'mvn test'
            }
        }
    }
}

