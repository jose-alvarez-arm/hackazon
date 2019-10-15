pipeline {
  agent any
  stages {
    stage('building binary') {
      steps {
        build 'echo \'Building\''
      }
    }
    stage('') {
      steps {
        snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'Hackazon', snykInstallation: 'Snyk')
      }
    }
  }
}