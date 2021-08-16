pipeline{
  agent any
  stages{
    stage("build"){
      steps{
        echo "building an application-webhook"
        script{  def exp=2+2>3 ? 'true' : 'incorrect'
        }
      }
    }
    stage("test"){
      steps{
        echo "testing the application"
      }
    }
    stage("deploy"){
      steps{
        echo "deploy the application"
      }
    }
  }
}
