pipeline {
    agent any

    stages {
	    stage('Testing')
	    {
		    steps{
			    echo "Testing ...."
		    }
	    }
        stage('Build') {
            steps {
                bat 'mvn clean package'
		bat "docker build . -t mywebapp:${env.BUILD_ID}"
            }
        }
     }
}
