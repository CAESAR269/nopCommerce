pipeline {
  agent { label 'Docker' }
  stages {
    stage('vcs'){
      steps {
      git branch: 'develop',
          url: 'https://github.com/CAESAR269/nopCommerce.git'
      }
    }
    stage('build'){
      steps {
        sh ' docker build -f Dockerfile --tag nopcommerce .'
      }
    }
  }
}
