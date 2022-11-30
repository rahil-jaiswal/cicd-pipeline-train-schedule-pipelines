pipeline{
  agent any
  stages{
    stage('Build') {
      steps{
        echo 'Building...'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
