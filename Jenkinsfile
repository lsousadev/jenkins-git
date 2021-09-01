pipeline {
  agent { docker { image 'python:3.5.1'} }
  stages {
    stage('Build branch') {
      environment {
          stage = "dev"
          tag = "latest"
      }
      steps {
                sh 'echo "HELLO"'
      }
    }
  }
}
