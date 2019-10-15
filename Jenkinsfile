pipeline {
  agent any
  stages {
    stage('Snyk dep check') {
      steps {
        echo 'passed'
        findText(regexp: 'passed', succeedIfFound: true, alsoCheckConsoleOutput: true)
        snykSecurity(snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a', snykInstallation: 'Snyk', projectName: 'hackazon', organisation: 'jose-alvarez-arm')
      }
    }
  }
}