node {
    stage('Checkout') {
        checkout([$class: 'GitSCM',
                  branches: [[name: '*/master'], [name: '*/ninja']],
                  extensions: [],
                  userRemoteConfigs: [[url: 'https://github.com/ritesh107/springhub.git']]])
    }
    
    stage('Build') {
        steps {
            sh 'mvn clean package'
        }
    }
    
    stage('Test') {
        steps {
            sh 'mvn test'
        }
    }
    
    stage('Deploy') {
        steps {
            echo "Deploy"
        }
    }
}
