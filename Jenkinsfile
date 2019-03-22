pipeline {
    agent any
    stages {
        stage('build') {
			environment {
				SONAR_HOST_URL = 'http://10.0.15.17:9000'
				sonarEnv = 'MaryanSonar'
			}
			steps {
				withSonarQubeEnv(sonarEnv) {
					sh './gradlew --info sonarqube'
				}  
			}
        }
    }
}

