pipeline {
  agent {
    docker {
      image 'benhall/dind-jenkins-agent'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t jpss/petclinic .'
        sh './mvnw package'
      }
    }

  }
}