pipeline {
agent any
  stages {
    stage ('build') {
      steps {
        echo 'the build stage will begin'
        sh './gradlew build --no-daemon' 
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
