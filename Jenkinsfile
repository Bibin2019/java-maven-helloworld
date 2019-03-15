pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
                 
            }
        }
    }
}
