#!groovy
pipeline {
	agent docker
  stages {
  	stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:3.5.0'
        }
      }
      steps {
        sh 'which docker'
      	sh 'mvn clean install'
      }
    }
  }
}
