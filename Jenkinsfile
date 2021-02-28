pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
      args '-v /root/.m2:/root/.m2'
    }

  }
  stages {
    stage('Bulid') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }

  }
}