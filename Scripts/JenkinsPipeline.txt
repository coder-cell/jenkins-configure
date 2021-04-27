pipeline {
    agent {label 'Mars'}
    stages {
          stage('Unit Test') {
             steps {
                echo 'Unit Testing Done.'
             }
          }
          stage('Integration Test') {
             steps {
                echo 'Integration Testing Done.'
             }
          }
          stage('System Test') {
             steps {
                echo 'System Testing Done.'
             }
          }
          stage('Acceptance Test') {
             steps {
                echo 'Acceptance Testing Done.'
             }
          }
       }
}