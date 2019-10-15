pipeline {
  agent any
  stages {
    stage('set non zero ') {
      steps {
        catchError(buildResult: '!0', stageResult: 'Stable', catchInterruptions: true)
      }
    }
    stage('Snyk dep check') {
      steps {
        snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'hackazon', snykInstallation: 'Snyk')
      }
    }
  }
}