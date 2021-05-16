pipeline {
  agent {
    docker {
      image 'python:3.7-alpine'
    }

  }
  stages {
    stage('Test') {
      steps {
          emailext body: 'Running Mount-Fuji script',
                subject: 'Mount Fuji Starting',
                     to: 'subhashrehan@gmail.com'
        sh 'python3 main.py'
      }
    }

  }
}
