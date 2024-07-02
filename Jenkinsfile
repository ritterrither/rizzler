pipeline {
    agent any
    stages {
        stage('No-op') {
            steps {
                sh 'ls'
            }
        }
    }
    post {
        failure {
        mail to: 'rither.le@avepoint.com',
             subject: "Failed Pipeline",
             body: "Something is wrong with the build urgh smh"
    }
    }
}
