pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('Bulid') {
      steps {
        sh 'mvn clean package'
      }
    }

  }
}