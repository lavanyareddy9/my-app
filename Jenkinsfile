pipeline {
  agent any
  stages{
    stage("SCM Checkout"){
      steps{
        git credentialsId: 'lavanyareddy9', url: 'https://github.com/lavanyareddy9/my-app', branch: "master"
      }
    }
    stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
  }
}
