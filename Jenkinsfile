pipeline {
  agent any
  stages {
    stage ('Artifact') {
      script {
        archiveArtifacts artifacts: 'output.txt', fingerprint: true
      }
    }
  }
}
