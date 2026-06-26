pipeline {
    agent any
    tools {
    sonarRunner 'sonar-scanner'
    }
    stages {
        stage('SonarQube Analysis') {
            steps {
                withSonarQubeEnv('sonarqube') {
                    sh 'sonar-scanner'
                }
            }
        }
    }
}
