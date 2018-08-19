pipeline {
  agent {
    docker {
      image 'mozart/grails/'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'grails prod build-standalone --jetty ropeytasks.jar'
      }
    }
  }
}