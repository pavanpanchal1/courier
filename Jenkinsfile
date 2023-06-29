pipeline {
    agent any
    
    environment {
        staging_server = "185.27.134.11"
    }
    
    stages {
        stage('Deploy') {
            steps {
                sh "scp -r ${WORKSPACE}/* root@${staging_server}:htdocs/"
            }
        }
    }
}
