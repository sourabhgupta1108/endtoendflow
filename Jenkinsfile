


pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build app'
            }
        }
        stage('Test') {
            steps {
                echo 'Test app'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy app'
            }
        }
    }
    post {
        always
        {
            emailext body: '''Hello, This is pipeline status. Thanks''', subject: 'pipeline status', to: 'sourabhgupta1108@gmail.com'
        }
    }
}
