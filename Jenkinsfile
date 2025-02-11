pipeline {
  agent {
    label 'jenkins'
  }
  stages {
    stage('Build') {
      steps {
        sh '''
        echo "Starting hello World pipeline"
        javac Hello.java
        '''
      }
    }
    stage('Execute') {
      steps {
        sh '''
        java Hello
        '''
      }
    }
  }
}
