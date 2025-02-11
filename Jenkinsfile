pipeline {
  agent {
    label 'jenkins'
  }
  stages {
    stage('Build') {
      steps {
        bat '''
        echo Starting hello World pipeline
        javac main.java
        '''
      }
    }
    stage('Execute') {
      steps {
        bat '''
        java main
        '''
      }
    }
  }
}
