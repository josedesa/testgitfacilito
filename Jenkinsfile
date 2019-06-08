pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Hello World! tet ${GIT_BRANCH}  ,  ,  ${BUILD_NUMBER} ,   ${BUILD_URL}  ,  "
                
            }
        }
        stage('Create Artifact 2') {
		  steps {
			sh 'tar -czvf frontend-${BUILD_NUMBER}.tar.gz ../testpipe/test.txt'
		  }
		}
	     stage('Deploy') {
			  steps {
				sh 'ansible servers -m ping -i inventory.ini'
				
			}
	     }
    
    }
}
