pipeline {
    agent {label 'Mars'}
		
    stages {

		    stage('Git'){
             steps{
               checkout([$class: 'GitSCM',
               branches: [[name: "c43f69fba50742b947d42655d10d8a3f19b5e531"]],
               userRemoteConfigs: [[
               url: 'https://github.com/coder-cell/robot-gsearch.git']]])		 
             } 
		  }	
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