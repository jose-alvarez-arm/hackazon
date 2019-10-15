pipeline {
  agent any
  stages {
    stage('Snyk Dep Check') {
      steps {
        snykSecurity(projectName: 'Hackazon', snykTokenId: 'snyk-token', snykInstallation: 'Snyk', organisation: 'jose-alvarez-arm', severity: 'low')
      }
    }
  }
}