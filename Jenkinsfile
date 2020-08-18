pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t jpss/petclinic .'
        sh './mvnw package'
      }
    }

  }
}