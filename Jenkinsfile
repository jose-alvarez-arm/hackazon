pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'Hackazon', snykInstallation: 'Snyk', snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a')
      }
    }
  }
}