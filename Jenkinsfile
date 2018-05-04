pipeline {
  agent {
    dockerfile {
      filename 'bjhbj'
    }

  }
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
  }
}