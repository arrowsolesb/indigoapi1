pipeline {
  agent any
  stages {
    stage('Build Application') { 
    	steps{
        	bat 'mvn clean install'
        }
    }
    stage('Deploy Mule Application into Cloud') { 
    	steps{
        	bat 'mvn package deploy -DmuleDeploy'
        }
    }
  }
    
}