pipeline {
  agent any
  stages {
    stage('Checkout'){
      steps {
        checkout scm
      }
    }
    stage('Compile blueprint') {
      steps {
        script{
          docker.image('ntnx/calm-dsl').inside{
            'calm'
          }
        }
      }
    }

  }
}