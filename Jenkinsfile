pipeline {
  agent any
  stages {
    stage ('Checkout'){
      steps {
        checkout scm
      }}
  stage ('Build'){
  steps {
    echo 'Running Build Automation'
    sh './gradlew build --no-daemon'
    archiveArtifacts artifacts: 'dist/sampleapp.zip'
    }
   }
  }
}
