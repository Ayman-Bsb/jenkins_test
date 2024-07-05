pipeline {
    agent any

    options {
        timeout(time: 1, unit: "HOURS")
    }

    stages {
        stage('build') {
            options {
                timestamps()
            }
            steps {
                echo 'Build application ...'
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