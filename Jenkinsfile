pipeline {
    agent {
        docker { image 'python:3.7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                mail body: 'project build successful',
                     from: 'subhashrehan@gmail.com',
                     replyTo: 'subhashrehan@gmail.com',
                     subject: 'project build successful',
                     to: 'subhashrehan@gmail.com'
                
                sh 'python3 main.py'
            }
        }
    }
}
