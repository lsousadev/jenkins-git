pipeline {
  agent { docker { image 'python:3.5.1' } }
  stages {
    stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
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
