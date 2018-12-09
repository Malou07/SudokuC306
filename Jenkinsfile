pipeline {
  agent any
  stages {
    stage('check') {
      steps {
        checkstyle(canComputeNew: true)
      }
    }
  }
}