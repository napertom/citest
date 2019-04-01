pipeline {
agent any
stages {
stage('compile stage') {
steps {
withMaven(maven : 'M3') {
sh 'mvn clean compile'
}
}
}
}

stages {
stage('test stage') {
steps {
withMaven(maven : 'M3') {
sh 'mvn test'
}
}
}
}

stages {
stage('deployment stage') {
steps {
withMaven(maven : 'M3') {
sh 'mvn deploy'
}
}
}
}
}
