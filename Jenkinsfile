pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        build(waitForStart: true, job: 'Clean')
        archiveArtifacts(artifacts: 'App', allowEmptyArchive: true)
      }
    }

  }
  environment {
    Build = 'test'
  }
}