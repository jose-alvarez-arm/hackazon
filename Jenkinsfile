pipeline {
  agent any
  stages {
    stage('') {
      steps {
        snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'Hackazon', severity: 'low', snykInstallation: 'Snyk', snykTokenId: 'snyk-token')
      }
    }
  }
}