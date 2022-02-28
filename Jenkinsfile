pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building ...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test one ...'
          }
        }

        stage('Test two') {
          steps {
            echo 'Test two ...'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}