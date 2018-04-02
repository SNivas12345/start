pipeline {
  agent {
    node {
      label 'nodeapp.prod'
    }
    
  }
  stages {
    stage('input') {
      parallel {
        stage('input') {
          steps {
            sh 'start'
          }
        }
        stage('process') {
          steps {
            sh 'find'
          }
        }
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'intialize'
          }
        }
        stage('manage') {
          steps {
            sh 'work'
          }
        }
      }
    }
  }
}