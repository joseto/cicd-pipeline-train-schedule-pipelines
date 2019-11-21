pipeline {
  agent any
  stages {
    stage ("Build") {
      steps {
        echo 'Corriendo la automatizacion'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
