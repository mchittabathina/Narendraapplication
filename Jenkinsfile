pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/mchittabathina/Narendraapplication.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
    stage('sonarqube') {
      steps {
        bat 'mvn sonar:sonar'
        bat 'mvn sonar:sonar'
      }
    }
  }
}