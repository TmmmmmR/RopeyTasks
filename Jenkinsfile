pipeline {
  agent {
    docker {
      image 'grails mozart/grails:3'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''grails prod build-standalone --jetty ropeytasks.jar
'''
      }
    }
  }
}