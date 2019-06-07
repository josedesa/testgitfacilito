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
            sh 'tar -czvf /tmp/frontend-${BUILD_NUMBER}.tar.gz index.html'
           }
        }
        
        
        
    }
}
