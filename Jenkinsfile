node {
    
     stage('Checkout') {
        checkout scm
    }
    
    stage('Build') {
        steps {
        bat 'mvn clean'
      }
    }
}
