pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh 'export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.20.0.8-1.el7_9.x86_64/'
                sh './gradlew build --no-daemon '
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
