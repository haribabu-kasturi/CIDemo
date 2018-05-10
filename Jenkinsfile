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
    stage('print') {
      steps {
        echo 'hello'
      }
    }
    stage('Sleep') {
      steps {
        sleep 20
      }
    }
  }
}