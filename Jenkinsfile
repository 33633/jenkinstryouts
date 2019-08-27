pipeline {
    agent any
    stages {
        stage('clean') {
            steps {
                tool name: 'maven', type: 'maven'
                sh "${tool name: 'maven', type: 'maven'}/bin/mvn clean"
            }
        }
        stage('test') {
            steps {
                tool name: 'maven', type: 'maven'
                sh "${tool name: 'maven', type: 'maven'}/bin/mvn test"
            }
        }
        stage('package') {
            steps {
                tool name: 'maven', type: 'maven'
                sh "${tool name: 'maven', type: 'maven'}/bin/mvn package"
        }
     }
  }
}
