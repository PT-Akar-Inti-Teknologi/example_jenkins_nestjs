pipeline {
  agent any

  stages {
    stage('Build') {
      agent {
        docker {
          image 'node:14-alpine'
        }
      }
      steps {
        sh 'npm install --force'
      }
    }

//     stage('Sonarqube') {
//       environment {
//         scannerHome = tool 'sonarqube-scanner'
//       }

//       steps {
//         withSonarQubeEnv(installationName: 'sonarqube') {
//           sh "${scannerHome}/bin/sonar-scanner"
//         }
//       }
//     }

  }
}
