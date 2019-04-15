pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh './gradew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true                
            }
        }
   }
}
