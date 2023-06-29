pipeline{
    agent any
    environment{
        staging_server="185.27.134.11"
    }
    stages{
        stage(''){
            steps{
                sh 'scp ${WORKSPACE}/* root@${staging_server}:htdocs/'
            }
        }
    }
}