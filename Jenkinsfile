pipeline {
  agent any
  stages {
    stage('Snyk Dep Check') {
      steps {
        snykSecurity(projectName: 'hackazon', snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a', snykInstallation: 'Snyk', organisation: 'jose-alvarez-arm', failOnIssues: true, targetFile: 'hackazon/blob/hackazondev/composer.lock')
      }
    }
  }
}