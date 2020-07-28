pipeline {
  agents any

  stages {
    stage ('Build') {
      steps {
        sh 'echo "Running gradle wrapper build"'
        sh './gradlew build --no-deamon'
        archiveArtifacts 'dist/trainSchedule.zip'
      }
    }
  }
}
