pipeline {
  agent any
  stages {
    stage('Install Dependencies') {
      steps {
        slackSend color: '#f7a54a', message: "Build Started - ${NAME} ${BUILD_NUMBER} (<${BUILD_URL}|Open>)"
        dir(path: 'frontend') {
          sh 'npm install'
        }

      }
    }
  }
}
