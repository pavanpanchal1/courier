pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                sh "scp -r ${WORKSPACE}/* root@myproject.000.pe:/htdocs/"
            }
        }
    }
}
