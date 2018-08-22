/*
** Demo DevSecOps **
*/

node {
      stage('Checkout') {
      steps {
        sh 'echo "X Step"'
      }
   }
   
   stage('Build') {
      steps {
        sh 'echo "X Step"'
      }
   }
   
  stage('Tests') {
      steps {
        parallel(
          "Unit Tests": {
            sh 'echo "Unit Tests"'
            
          },
          "Feature tests": {
            sh 'echo "Feature Tests"'
          }
        )
      }
  }

   stage("Results"){
      steps {
        sh 'echo "X Step"'
      }
   }
   
   
   //Get approval from user before deployment
    input 'Ready to Deploy??'

    stage("Deploy"){
      steps {
        sh 'echo "X Step"'
      }
    }
}
