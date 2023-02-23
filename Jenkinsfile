pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'First Dev'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test nvironment'
          }
        }

        stage('test1') {
          steps {
            echo 'test1'
          }
        }

      }
    }

    stage('Deployment') {
      steps {
        echo 'Deploying stage'
      }
    }

  }
}