pipeline {
    agent any
    stages {
        stage('Docker CentOS') {
            agent { docker 'centos' } 
            steps {
                echo 'Hello, CentOS Linux'
                sh 'uname -a'
                sh 'id'
                sh 'date'
            }
        }
    }
}
