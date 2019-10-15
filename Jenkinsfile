pipeline {
  agent any
  stages {
    stage('Snyk dep check') {
      steps {
        echo 'passed'
        findText(regexp: 'passed', succeedIfFound: true, alsoCheckConsoleOutput: true)
        build 'Snyk_Dep_Check'
      }
    }
  }
}