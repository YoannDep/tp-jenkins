pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'composer update'
      }
    }
    stage('Test Laravel') {
      steps {
        sh '''composer require phpunit/phpunit --dev 
composer global install phpunit/phpunit'''
      }
    }
  }
}