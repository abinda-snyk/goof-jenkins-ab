pipeline {
  agent any

  stages {
    stage('Node') {
      steps {
        sh 'npm install'
      }
    }
    stage('Snyk') {
      steps {
        snykSecurity(failOnIssues: true, snykInstallation: 'Snyk')
      }
    }
  }
}