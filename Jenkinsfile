pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        warnError(message: 'Snyk issues found')
      }
    }
    stage('Synk Dep check') {
      steps {
        snykSecurity(snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a', snykInstallation: 'Snyk', projectName: 'hackazon', organisation: 'jose-alvarez-arm')
      }
    }
  }
}