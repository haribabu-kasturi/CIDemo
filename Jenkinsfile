pipeline {
  agent any
  stages {
    stage('Sleep') {
      steps {
        sleep 2
      }
    }
    stage('printing message') {
      steps {
        echo 'I am testing'
      }
    }
    stage('email users') {
      steps {
        mail(subject: 'for testing', body: 'lorem ipsum etc', to: 'dinesh.pahi@cgi.com', from: 'anuradha.bhattacharya@cgi.com', charset: 'UTF', mimeType: 'text')
      }
    }
  }
}