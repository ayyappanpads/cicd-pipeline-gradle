pipeline {
  agent any
  stages {
    Stage ('Checkout'){
      steps {
        checkout Scm
      }}
Steps
  stage ('Build'){
  steps {
    echo 'Running Build Automation'
    sh './gradlew build --no-daemon'
    archiveArtifacts artifacts: 'dist/sampleapp.zip'
    }
   }
  }
}
