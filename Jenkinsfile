pipeline {
  agent any
  stages {
    stage('POS Sales') {
      steps {
        echo 'Add Item'
      }
    }

    stage('POS Print') {
      parallel {
        stage('Select Done') {
          steps {
            echo 'Print Receipt'
          }
        }

        stage('Close Transaction') {
          steps {
            sh 'echo done'
          }
        }

      }
    }

  }
}