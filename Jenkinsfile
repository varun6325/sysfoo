pipeline {
  agent {
    docker {
      image 'maven:3.6.3-jdk-11-slim'
    }

  }
  stages {
    stage('build') {
      steps {
        echo 'compile sysfoo app'
        sh 'mvn compile'
      }
    }

    stage('test') {
      steps {
        echo 'compile sysfoo app'
        sh 'mvn test'
      }
    }

    stage('package') {
      steps {
        echo 'compile sysfoo app'
        sh 'mvn package -DskipTests'
      }
    }

  }
  tools {
    maven 'maven 3.6.3'
  }
}