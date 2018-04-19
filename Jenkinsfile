pipeline {
  agent any
  stages {
    stage('Verify Sanity') {
      steps {
        sh '''echo "Starting the build now" 
'''
        sleep 20
        mail(subject: 'Starting Build', body: 'hei and hello ', charset: 'UTF', from: 'jenkins@ci.com', mimeType: 'Plaintext', to: 'haribabu.kasturi@cgi.com')
      }
    }
    stage('Code Quality Verification ') {
      steps {
        sh 'echo "Running SonarCube" '
      }
    }
    stage('Test on firefox') {
      parallel {
        stage('Test on firefox') {
          steps {
            sh 'echo "Testing on firefox" '
          }
        }
        stage('Test on chrome ') {
          steps {
            sh 'echo "Test on Chrome" '
          }
        }
        stage('Test on Opera ') {
          steps {
            sh 'echo "Test on Opera" '
          }
        }
      }
    }
    stage('Deploy ') {
      steps {
        sh 'echo "create environment" '
      }
    }
  }
}