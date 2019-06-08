pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Hello World! ${GIT_BRANCH}  ,  ,  ${BUILD_NUMBER} ,   ${BUILD_URL}  ,  "
                
            }
        }
        stage('Create Artifact') {
      steps {
        sh 'tar -czvf /tmp/frontend-${BUILD_NUMBER}.tar.gz dist'
      }
    }
        environment {
    NAME = "frontend/${GIT_BRANCH}"
    DEPLOY_TARGET = "frontend-${GIT_BRANCH}"
    DEPLOY_PATH = '/var/www/frontend'
    PRIVATE_KEY = "/root/.ssh/masonfinance.pem"

  }
        
        
        
    }
}
