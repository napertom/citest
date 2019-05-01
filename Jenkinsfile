pipeline {
    agent none
    stages {
        stage('Example Build') {
            agent { docker 'centos' } 
            steps {
                echo 'Hello, Linux'
                sh 'gcc --version'
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
