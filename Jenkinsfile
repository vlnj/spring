node {
    
     stage('Checkout') {
        checkout scm
    }
    
    stage('Build') {
        bat 'mvn clean install'
    }
    
    stage('Post'){
        def response = httpRequest "http://localhost:6029/configar-api/test"
        println('Status: '+response.status)
        println('Status: '+response.content)
    }
}
