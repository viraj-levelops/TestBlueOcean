pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build'
      }
    }

    stage('Unit Tests') {
      steps {
        echo 'Unit Tests'
      }
    }

    stage('Package') {
      steps {
        echo 'Package'
      }
    }

    stage('Deploy Stg1') {
      parallel {
        stage('Deploy Stg1') {
          steps {
            echo 'Deploy Stg1'
          }
        }

        stage('Deploy Stg2') {
          steps {
            echo 'Deploy Stg2'
          }
        }

        stage('Deploy Stg3') {
          steps {
            echo 'Deploy Stg3'
          }
        }

      }
    }

    stage('Deploy Prod') {
      steps {
        echo 'Deploy Prod'
      }
    }

  }
}