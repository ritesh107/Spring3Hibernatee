node {
    agent any
    stages ('clone & Checkout') {
        steps {
            bat "git clone https://github.com/ritesh107/springhub.git"
    }
    
    stage('install') {
        steps {
            bat "mvn install"
        }
    }
    
    stage('Test') {
        steps {
            bat "mvn test"
        }
    }
    
    stage('package') {
        steps {
            bat "mvn package"
        }
    }
}
