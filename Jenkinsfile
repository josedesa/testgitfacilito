pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Hello World! ${GIT_BRANCH}  ,  ${NAME} ,  ${BUILD_NUMBER} ,   ${BUILD_URL}  ,  ${DEPLOY_TARGET}  "
            }
        }
         stage('Create Artifact') {
         steps {
            sh 'ls'
           }
        }
        
        
        
    }
}
