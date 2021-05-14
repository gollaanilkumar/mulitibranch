pipeline{
  agent any
  stages{
    stage("deploy to dev"){ 
     when {
        branch "dev"
      }
 steps{
        echo "deploy to dev environment"
      }   
      }
    }
    stage ("deploy to preprod")
    {
      when{
        branch "preprod"

      }
     steps{
        echo "deploy to preprod environment"
      }   
    }
   stage ("deploy to prod")
    {
      when{
        branch "main"
      }
     steps{
        echo "deploy to prod environment"
      }   
    } 
  }
}
