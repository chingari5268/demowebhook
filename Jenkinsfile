pipeline {
  agent any
  stages {
    stage('Checkout Source') {
      steps {
        git branch: 'main', url: 'https://github.com/chingari5268/demowebhook.git'
      }
    }
     stage('Hello') {
            steps {
                echo 'Hello World chethan monday!'
            }
        }
    }
}
