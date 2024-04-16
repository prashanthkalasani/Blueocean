pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        echo 'commit the code'
      }
    }

    stage('build') {
      steps {
        echo 'build the code'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test the code'
          }
        }

        stage('stage') {
          steps {
            echo 'stage the code'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the code'
          }
        }

        stage('operate') {
          steps {
            echo 'operate the code'
          }
        }

      }
    }

  }
}