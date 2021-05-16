pipeline {
    agent {
        docker { image 'python:3.7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                        def message = "hello there!" 

                        mail bcc: '', body: message, cc: '', from: 'jenkinsuser@mycom.com', replyTo: 'jenkinsuser@mycom.com', subject: "Develop: build starting ",     to:'subhashrehan@gmail.com'
                
                sh 'python3 main.py'
            }
        }
    }
}
