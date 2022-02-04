pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building***'
      }
    }

    stage('Firefox') {
      parallel {
        stage('Firefox') {
          steps {
            echo 'Testing Firefox'
          }
        }

        stage('Edge') {
          steps {
            echo 'Testing Nioh 2...'
          }
        }

        stage('Safari') {
          steps {
            echo 'Testing Safari ==='
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Done, now ready to deploy"'
      }
    }

  }
}
