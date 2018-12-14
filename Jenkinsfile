pipeline {
  agent any
  stages {
    stage('check') {
      parallel {
        stage('check') {
          steps {
            checkstyle(canComputeNew: true)
          }
        }
        stage('findbugs') {
          steps {
            catchError()
          }
        }
      }
    }
    stage('cobertura') {
      steps {
        cobertura(autoUpdateHealth: true)
      }
    }
  }
}