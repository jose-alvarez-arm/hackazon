pipeline {
  agent any
  stages {
    stage('Snyk dep check') {
      parallel {
        stage('Snyk dep check') {
          steps {
            snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'hackazon', snykInstallation: 'Snyk', snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a')
          }
        }
        stage('non zero') {
          steps {
            findText(regexp: 'issues', succeedIfFound: true, unstableIfFound: true, alsoCheckConsoleOutput: true)
          }
        }
      }
    }
  }
}