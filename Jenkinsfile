pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew wrapper --gradle-version 6.0.1'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
