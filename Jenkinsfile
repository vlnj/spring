pipeline {
  agent {
    node {
      label 'rest'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        bat 'mvn clean'
      }
    }
  }
}