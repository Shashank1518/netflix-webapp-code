pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/devopsbyraham/jenkins-java-project.git', branch: 'master')
      }
    }
    stage('Build, Test, Deploy') {
      steps {
        bat 'mvn clean package'
      }
    }
  }
}
