pipeline {
  agent any
  stages {
    stage('Testing') {
      steps {
        echo 'running Tests'
        sh 'mvn test'
      }
    }
    stage('Build') {
      steps {
        echo 'Building jar files...'
        sh 'mvn package'
      }
    }
  }
  tools {
        maven 'Maven 3.8.5'
  }
}
