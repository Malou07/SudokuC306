pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        checkstyle(canComputeNew: true)
      }
    }
    stage('cobertura') {
      steps {
        cobertura(autoUpdateHealth: true)
      }
    }
  }
}