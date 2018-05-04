pipeline {
  agent any
  stages {
    stage('Sleep ') {
      steps {
        sleep 2
      }
    }
    stage('error') {
      steps {
        echo 'Hello'
      }
    }
    stage('email') {
      steps {
        mail(subject: 'testing', body: 'testing', from: 'anuradha.bhattacharya@cgi.com', mimeType: 'text', to: 'mrinmoy.nath@cgi.com')
      }
    }
  }
}