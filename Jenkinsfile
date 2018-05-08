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
    stage('email') {
      steps {
        mail(subject: 'test', body: 'testing', from: 'swakriti.kumari@cgi.com', mimeType: 'text', to: 'anuradha.bhattacharya@cgi,com')
      }
    }
  }
}