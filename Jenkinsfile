pipeline {
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
