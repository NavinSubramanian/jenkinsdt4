pipeline {
  agent {
    label 'jenkins_agent'
  }
  environment {
    PATH = "/usr/bin:$PATH"
    SHELL = "/bin/bash"
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
