pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package dockerfile:build -DskipTests'
      }
    }
  }
}