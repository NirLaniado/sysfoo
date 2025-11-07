pipeline {

  agent any

  tools {
    maven 'mvn'
  }
  
  stages {

    stage('Build') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn clean test'
      }
    }

    stage('Package') {
      steps {
        sh 'mvn package -DskipTests'
      }
    }
  }
}
