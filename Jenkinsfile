pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradle wrapper build --no-daemon '
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
