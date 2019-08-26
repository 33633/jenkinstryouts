pipeline {
    agent any
    stages {
        stage('clean') {
            tool name: 'maven', type: 'maven'
            steps {
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
