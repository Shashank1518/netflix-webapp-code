pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git 'https://github.com/devopsbyraham/jenkins-java-project.git'
      }
    }
    stage('Build, Test, Deploy') {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
