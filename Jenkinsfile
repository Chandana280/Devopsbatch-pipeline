pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'i have a plan'
      }
    }

    stage('Code') {
      steps {
        echo 'i have a ode'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'i have a build'
          }
        }

        stage('test') {
          steps {
            echo 'i have tested'
          }
        }

        stage('release') {
          steps {
            echo 'i have a release'
          }
        }

        stage('deploy') {
          steps {
            echo 'i have deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'i have operate'
          }
        }

      }
    }

  }
}