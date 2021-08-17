pipeline{
  agent any
  parameters{
    choice(name: 'version', choices:['1.2','1.34','1.45'], description:'check the choice')
    booleanParam(name: 'install', defaultValue=true)
  }
  tools{
    maven 'maven'
  }
  environment{
    NEW_VERSION='1.3.0'
    SERVER_CREDENTIALS=credentials('git')
  }
  stages{
    stage("build"){
      steps{
        echo "building an application-webhook added"
        script{  def exp=2+2>3 ? 'true' : 'incorrect'
        }
      }
    }
    stage("test"){
      steps{
        echo "testing the application"
        echo "credentials ${SERVER_CREDENTIALS}"
        
      }
    }
    stage("deploy"){
      steps{
        echo "deploy the application"
        echo"deploy version ${NEW_VERSION}"
        echo "adding line"
      }
    }
  }
}
