pipeline {
  agent any
  stages {
    stage('Dockerbuild') {
      steps {
        sh 'docker build -t server .'
      }
    }

    stage('Dockerrun') {
      steps {
        sh 'docker run -d -p 3000:3000 server'
      }
    }

  }
}