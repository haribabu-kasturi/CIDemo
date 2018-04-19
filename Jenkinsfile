pipeline {
  agent any
  stages {
    stage('testing') {
      steps {
        jiraSearch 'project = ASDCUNIFY AND issuetype = Epic AND text ~ "configure"'
        sleep 10
      }
    }
    stage('email to stakeholders') {
      steps {
        emailext(subject: 'For testing purpose', body: 'lorem ipsum', from: 'anuradha.bhattacharya@cgi.com', mimeType: 'text', to: 'dinesh.pahi@cgi.com')
        timestamps() {
          echo 'this pipeline is for testing'
        }

      }
    }
  }
}