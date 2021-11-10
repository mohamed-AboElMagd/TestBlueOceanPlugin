pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
        retry(count: 3) {
          sh 'wwwwwww'
        }

      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test1 completed'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2 completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you wanna deploy?', ok: 'yes, I\'m Sure')
        echo 'Deployment Completed'
      }
    }

    stage('Notify for new Build') {
      steps {
        echo 'Build Completed '
      }
    }

  }
}