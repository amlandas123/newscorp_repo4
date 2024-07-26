pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      agent any
      steps {
        echo 'SCM Stage successfull'
      }
    }

    stage('Deploy_Dev') {
      parallel {
        stage('Deploy_Dev') {
          agent any
          steps {
            echo 'Deploy_dev Successfull'
          }
        }

        stage('Deploy_QA') {
          agent any
          steps {
            echo 'QA_successfull'
          }
        }

      }
    }

    stage('Deploy_Prod') {
      agent any
      steps {
        echo 'Prod_Successfull'
      }
    }

  }
}