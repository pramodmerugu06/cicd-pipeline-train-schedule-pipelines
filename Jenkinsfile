pipeline{
    agent any
    stages {
        stage(Build) {
            steps {
                echo "Running build automation"
                sh './gradlew build --no-daemon'
            }
        }
        stage (Archive) {
            steps {
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}    
