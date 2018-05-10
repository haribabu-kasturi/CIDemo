pipeline {
  agent any
  stages {
    stage('Sleep ') {
      parallel {
        stage('Sleep ') {
          steps {
            sleep 10
          }
        }
        stage('Sleep1') {
          steps {
            echo 'Sleep1'
          }
        }
      }
    }
    stage('email') {
      steps {
        mail(subject: 'testing', body: 'testing', from: 'anuradha.bhattacharya@cgi.com', mimeType: 'text', to: 'mrinmoy.nath@cgi.com')
        echo 'Test'
      }
    }
    stage('print') {
      steps {
        echo 'hello'
      }
    }
  }
}