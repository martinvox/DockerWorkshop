pipeline {
  agent any
  stages {
    stage('Dockerbuild') {
      steps {
        sh 'sudo docker build -t server .'
      }
    }

    stage('Dockerrun') {
      steps {
        sh 'sudo docker run -d -p 3000:3000 server'
      }
    }

  }
}