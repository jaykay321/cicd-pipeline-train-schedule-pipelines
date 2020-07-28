pipeline {
  agent any

  stages {
    stage ('Build') {
      steps {
        sh 'echo "Running gradle wrapper build"'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }
  }
}
