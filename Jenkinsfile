pipeline {
  agent any
  
  environment {
    MY_MESSAGE = "Rafael"
  }
  
  stages {
    stage("echo some variable") {
      echo "ola, ${MY_MESSAGE}!"
    }
  }
  
  post {
    success {
      echo "parabens, foi um sucesso!!!!"
    }
    failure {
      echo "que pena, deu errado... :("
    }
  }
}
