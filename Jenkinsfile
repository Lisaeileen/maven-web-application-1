pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                git 'https://github.com/Lisaeileen/maven-web-application-1.git'
                sh 'ls -al'
            }
        }
        stage('Maven Package') {
            steps {
                echo "Packaging artifact using maven..."
                sh 'mvn clean package'
            }
        }
    }
}
