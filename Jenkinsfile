pipeline {
  agent any
  stages {
    stage('Cloning GIT') {
      steps {
        echo 'HI... This is build'
        git(url: 'https://github.com/Balu1819/hello-world.git', branch: 'master', credentialsId: 'balu1819')
        sh 'mvn package'
      }
    }

    stage('Build') {
      steps {
        echo 'This is Build'
        sh 'mvn clean package'
      }
    }

    stage('error') {
      steps {
        echo 'to generate docker image from Dockerfile'
        sh 'docker build .'
        sh 'pwd'
      }
    }

  }
}