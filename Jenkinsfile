pipeline {
  agent any
  stages {
    stage ('Artifact') {
      steps {
           script {
              archiveArtifacts artifacts: 'output.txt', fingerprint: true
         }
      }
    }
  }
}
