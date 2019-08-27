pipeline {
    agent any
    environment {
        mavn="${tool name: 'maven', type: 'maven'}/bin/mvn"
    }
    stages {
        stage('clean') {
            steps {
                sh "mavn clean"
            }
        }
        stage('test') {
            steps {
                sh "mavn test"
            }
        }
        stage('package') {
            steps {
                sh "mavn package"
        }
     }
  }
}
