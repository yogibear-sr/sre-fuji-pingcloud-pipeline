pipeline {
  agent {
    docker {
      image 'python:3.7-alpine'
    }

  }
  stages {
    stage('Test') {
      steps {
          emailext body: 'Test Message',
                subject: 'Test Subject',
                     to: 'subhashrehan@gmail.com'
        sh 'python3 main.py'
      }
    }

  }
}
