pipeline {
  agent { docker { image 'python:3.5.1'} }
  stages {
    stage('Build branch') {
      environment {
          when { branch 'develop' }
          stage = "dev"
          tag = "latest"
          when { branch 'master' }
          stage = "prod"
          tag = "$BUILD_NUMBER"
      }
      steps {
                sh 'echo "HELLO"'
      }
    }
  }
}
