pipeline {
  agent any
  stages {
    stage('Snyk dep check') {
      steps {
        snykSecurity(organisation: 'jose-alvarez-arm', projectName: 'hackazon', snykInstallation: 'Snyk', snykTokenId: '223a828a-794f-42cc-b3bb-df2f6d0d790a', additionalArguments: '--ignore --reason=\'Not currently exploitable.\'')
      }
    }
    stage('Scan results') {
      steps {
        findText(regexp: 'Archiving artifacts', alsoCheckConsoleOutput: true)
      }
    }
  }
}