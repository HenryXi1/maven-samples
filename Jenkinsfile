pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/HenryXi1/maven-samples.git', branch: 'master')
      }
    }

    stage('run test') {
      steps {
        sh 'mvn verify'
      }
    }

    stage('run verify') {
      steps {
        sh 'mvn verify'
      }
    }

    stage('run clean') {
      steps {
        sh 'mvn clean'
      }
    }

  }
}