pipeline {
    agent any

    tools {
        sonarQubeScanner 'sonar-scanner'
    }

    stages {

        stage('SonarQube Analysis') {
            steps {
                withSonarQubeEnv('SonarQube') {
                    sh 'sonar-scanner'
                }
            }
        }

    }
}
