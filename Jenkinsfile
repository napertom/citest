pipeline {
    agent none
    stages {
        stage('Example Linux') {
            agent { docker 'centos' } 
            steps {
                echo 'Hello, Linux'
                sh 'uname -a'
            }
        }
        stage('Example JDK') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
