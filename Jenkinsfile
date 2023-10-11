pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh 'export JAVA_HOME=/usr/lib/jvm/jre-11-openjdk'
                sh './gradlew build --no-daemon '
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
