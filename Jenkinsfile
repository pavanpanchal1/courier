pipeline {
    agent any
    
    environment {
        // staging_server = "185.27.134.11"
        staging_server = "https://filemanager.ai/new/#/c/185.27.134.11/if0_34518172/eyJ0IjoiZnRwIiwiYyI6eyJwIjoieVJLdXk3algxaSIsImkiOiIvIn19";
    }
    
    stages {
        stage('Deploy') {
            steps {
                sh "scp -r ${WORKSPACE}/* root@${staging_server}:/htdocs"
            }
        }
    }
}
