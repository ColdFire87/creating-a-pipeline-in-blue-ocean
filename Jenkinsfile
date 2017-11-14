pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:8.9.1'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
  environment {
    npm_config_cache = 'npm-cache'
  }
}