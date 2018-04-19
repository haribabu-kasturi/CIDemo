pipeline {
  agent any
  stages {
    stage('Search Jira Issue') {
      steps {
        jiraSearch 'ASCDUNIFY-24'
      }
    }
    stage('email to stakeholders') {
      steps {
        emailext(subject: 'For testing purpose', body: 'lorem ipsum', from: 'anuradha.bhattacharya@cgi.com', mimeType: 'text', to: 'dinesh.pahi@cgi.com')
      }
    }
  }
}