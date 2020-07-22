pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'HI... This is build'
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