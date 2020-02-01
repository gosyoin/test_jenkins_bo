pipeline {
  agent {
    node {
      label 'master_slave'
    }

  }
  stages {
    stage('Hello World') {
      steps {
        git(url: 'https://github.com/gosyoin/sikulix_vivid.git', branch: 'master')
        bat(script: 'sikulix_execute.bat', returnStatus: true, returnStdout: true)
      }
    }

  }
}