pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        echo 'Test Stage Successful'
      }
    }
    stage('Deploy'){
      steps{
        sh 'mvn edploy'
        echo 'Deploy Stage Successful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
