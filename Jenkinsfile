pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git url: 'https://github.com/Daiired/demo-app.git'
      }
    }
    stage('Compile & Test') {
      steps {
        bat 'mvn clean test'
      }
    }
    stage('Package') {
      steps {
        bat 'mvn package'
      }
    }
    stage('Deploy (simulado)') {
      steps {
        echo 'Desplegando artefacto...'
      }
    }
  }
}
