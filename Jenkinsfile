pipeline {
  agent {
    label 'jenkins'
  }
  environment {
    PATH = "C:\\WINDOWS\\SYSTEM32"
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
