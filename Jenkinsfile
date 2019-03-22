pipeline {
    agent any
    stages {
        stage('build') {
            environment {
	        SONAR_HOST_URL = http://10.0.15.17:9000
	    }
            steps {
		sh './gradlew --info sonarqube'  
            }
        }
    }
}

