pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build for Roberto'
        sh './gradlew build' --no-daemon
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
