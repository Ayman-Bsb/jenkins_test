pipeline {
    agent {
        docker {
            image 'node:22-alpine'
        }
    }

    stages {
        stage('build') {
            steps {
                sh 'npm -v'
            }
        }
    }

    post {
        always {
            echo 'always !'
        }
        success {
            echo 'success !'
        }
        failure {
            echo 'failure !'
        }
    }
}