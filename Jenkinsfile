pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Cloning GIT') {
          steps {
            echo 'HI... This is build'
            git(url: 'https://github.com/Balu1819/hello-world.git', branch: 'master', credentialsId: 'balu1819')
            sh 'mvn package'
          }
        }

        stage('Test') {
          steps {
            echo 'Hi This is Test'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'This is deploy'
      }
    }

    stage('Artifact') {
      steps {
        echo 'to store artifact'
      }
    }

  }
}