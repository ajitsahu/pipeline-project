pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'touch test.txt'
            }
        }
    }
    post {
        always {
           archiveArtifacts artifacts: 'Pipelint-project', fingerprint: true
        }
    }
}
