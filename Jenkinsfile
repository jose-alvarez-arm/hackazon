pipeline {
  agent any
  stages {
    stage('Snyk Dep Check') {
      steps {
        snykSecurity(organisation: 'arm', projectName: 'hackazon', snykTokenId: '0e474ca7-9325-4f22-bf6d-3b03ba869a4d', snykInstallation: '/usr/local/lib/node_modules/snyk')
      }
    }
  }
}