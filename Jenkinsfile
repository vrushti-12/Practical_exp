pipeline{
  agent any{
    stages{
      trigger("checkout"){
        checkout scm
        POLLSCM("H/5 * * * * ")
      }
      stage("build"){
        steps{
          echo "Application build successfully!"
        }
      }
      stage("Test"){
        steps{
          echo "Application Tested Successfully!"
        }
      }
    }
  }
