pipeline {
  agent { label 'DotNET' }
  stages {
    stage('vcs'){
      steps {
      git branch: 'develop'
          url: 'https://github.com/CAESAR269/nopCommerce.git'
      }
    }
    stage('build'){
      steps {
        sh 'dotnet build .nopCommerce/src/NopCommerce.sln'
      }
    }
  }
}
