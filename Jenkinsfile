pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
		bat "docker build . -t mywebapp:${env.BUILD_ID}"
            }
        }
     }
}
