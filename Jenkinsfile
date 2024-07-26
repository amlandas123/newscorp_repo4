pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM Stage successfull'
      }
    }

    stage('Deploy_Dev') {
      parallel {
        stage('Deploy_Dev') {
          steps {
            echo 'Deploy_dev Successfull'
          }
        }

        stage('Deploy_QA') {
          steps {
            echo 'QA_successfull'
          }
        }

      }
    }

    stage('Deploy_Prod') {
      steps {
        echo 'Prod_Successfull'
      }
    }

  }
}