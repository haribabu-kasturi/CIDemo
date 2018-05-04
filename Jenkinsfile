pipeline {
  agent any
  stages {
    stage('Sleep ') {
      steps {
        sleep 2
      }
    }
    stage('email') {
      steps {
        mail(subject: 'testing', body: 'testing', from: 'anuradha.bhattacharya@cgi.com', mimeType: 'text', to: 'mrinmoy.nath@cgi.com')
      }
    }
    stage('print') {
      steps {
        echo 'hello'
      }
    }
  }
}