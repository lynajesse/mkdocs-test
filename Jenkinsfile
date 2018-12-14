pipeline {
  agent any
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