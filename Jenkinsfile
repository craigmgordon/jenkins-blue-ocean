pipeline{
  agent none
  stages{
    stage('checkout'){
      agent any
      steps{
        echo 'checkout stage......'
      }
    }
    stage('build'){
      agent any
      steps{
        echo 'build stage......'
      }
    }
    stage('tests'){
      agent any
      steps{
        echo 'test stage......'
      }
    }
    stage('deploy to SIT'){
      agent any
      when {
          branch 'master' 
      }
      steps{
        echo 'SIT deploy stage......'
      }
    }
    stage('deploy to UAT'){
      agent any
      when {
          branch 'master' 
      }
      steps{
        echo 'UAT deploy stage......'
      }
    }
  }
}
