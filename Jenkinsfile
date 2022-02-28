pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('First Test') {
      parallel {
        stage('First Test') {
          steps {
            echo 'First Test...'
          }
        }

        stage('Second Test') {
          steps {
            echo 'Second Test...';
            exit 1
          }
        }

        stage('Third Test') {
          steps {
            echo 'Third Test...'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}
