pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'This is step 1'
        echo 'This is step 2'
      }
    }

    stage('stage 2') {
      parallel {
        stage('stage 2') {
          steps {
            echo 'This is step 1 from stage 2 '
          }
        }

        stage('stage 2A') {
          steps {
            echo 'This is step1 from stage 2A'
          }
        }

      }
    }

    stage('stage 3') {
      steps {
        echo 'This is step 1 from stage 3'
      }
    }

  }
}