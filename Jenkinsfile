pipeline {
  agent {
    docker {
      image 'squidfunk/mkdocs-material build'
      args '-v $WORSKPACE/ docs '
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''mkdocs build
ls -l _site/
'''
        sh '''mkdocs build
'''
      }
    }
  }
}