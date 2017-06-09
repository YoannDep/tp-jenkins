pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'composer install'
      }
    }
    stage('Test Laravel') {
      steps {
        sh '''composer require phpunit/phpunit --dev 
composer global install phpunit/phpu'''
      }
    }
  }
}