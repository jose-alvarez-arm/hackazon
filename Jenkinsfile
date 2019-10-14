pipeline {
  agent any
  stages {
    stage('Snyk Dep Check') {
      steps {
        snykSecurity(projectName: 'Hackazon', snykTokenId: '4861aad8-ac8f-4fb1-82a8-d02736f670f9', snykInstallation: '/usr/local/lib/node_modules', additionalArguments: 'sudo su ')
      }
    }
  }
}