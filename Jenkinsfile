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
      a: {
        echo "This is branch a"
      },
      b: {
        echo "This is branch b"
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
