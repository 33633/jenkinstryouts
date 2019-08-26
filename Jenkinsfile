pipeline {
    agent any
    stages {
        stage('clean') {
            steps {
                tool name: 'maven', type: 'maven'
                sh "mvn clean"
            }
        }
        stage('test') {
            steps {
                sh "mvn test"
            }
        }
        stage('package') {
            steps {
                sh "mvn package"
        }
     }
  }
}
