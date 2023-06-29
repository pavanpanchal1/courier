pipeline {
    agent any
    
    environment {
        staging_server = "http://myproject.000.pe/"
    }
    
    stages {
        stage('Deploy') {
            steps {
                sh "scp -r ${WORKSPACE}/* root@${staging_server}:/htdocs/"
            }
        }
    }
}
