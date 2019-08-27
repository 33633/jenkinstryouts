pipeline {
    agent any
    environment {
        mvn="${tool name: 'maven', type: 'maven'}/bin/mvn"
    }
    stages {
        stage('clean') {
            steps {
                sh "$mvn clean"
            }
        }
        stage('test') {
            steps {
                sh "$mvn test"
            }
        }
        stage('package') {
            steps {
                sh "$mvn package"
        }
     }
  }
}
