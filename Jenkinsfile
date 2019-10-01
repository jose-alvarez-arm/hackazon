pipeline {
  agent any
  stages {
    stage('Snyk Dep Check') {
      steps {
        snykSecurity(failOnIssues: true, monitorProjectOnBuild: true, organisation: 'arm', projectName: 'Snyk POC')
      }
    }
  }
}