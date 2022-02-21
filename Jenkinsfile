pipeline {
  agent any
  
  trigger {
    pollSCM('H/1 * * * *')
  }
  
  environment {
    MY_MESSAGE = 'Rafael'
  }
  
  stages {
    stage('echo some variable') {
      steps { 
        echo "ola, ${MY_MESSAGE}!"
      }
    }
  }
  
  post {
    success {
      echo 'parabens, foi um sucesso!!!!'
    }
    failure {
      echo 'que pena, deu errado... :('
    }
  }
}
