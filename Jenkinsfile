pipeline {
    agent any
    
    environment {
        staging_server = "example.infinityfreeapp.com"
    }
    
    stages {
        stage('Deploy') {
            steps {
                sh "scp -r ${WORKSPACE}/* root@${staging_server}:/htdocs/courierp/"
            }
        }
    }
}
