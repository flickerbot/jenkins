pipeline {
  agent any
  stages {
    stage('A') {
      parallel {
        stage('A') {
          steps {
            echo '========executing A========'
            input 'do you wanna continue '
            sh '''echo hello

'''
          }
        }

        stage('parallel') {
          steps {
            sleep 1
          }
        }

        stage('hello world ') {
          steps {
            echo 'hello bch'
          }
        }

      }
    }

    stage('SCript') {
      steps {
        sh '''pwd 
                ls
                     '''
      }
    }

  }
  post {
    always {
      echo '========always========'
    }

    success {
      echo '========pipeline executed successfully ========'
    }

    failure {
      echo '========pipeline execution failed========'
    }

  }
}