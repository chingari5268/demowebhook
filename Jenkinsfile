pipeline {
  agent any
  stages {
    stage('Checkout Source') {
      steps {
        git branch: 'main', url: 'https://github.com/chingari5268/demowebhook.git'
      }
    }
    stage('Manual approve') {
            steps {
                input 'Proceed or Abort'
            }
        }
     stage('trigger downstream jobs') {
            steps {
               build 'jesting'
            }
        }
    }
}
