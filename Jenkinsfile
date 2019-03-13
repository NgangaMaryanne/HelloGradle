pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                script {
                    withSonarQubeEnv('MaryanSonar') {
			sh './gradlew --info sonarqube'
                    } 
                }     
            }
        }
    }
}

