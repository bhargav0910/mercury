#!/usr/bin/env groovy

def VERSION
pipeline {

  agent none
  
  stage('Init Stage') {
    steps{
      VERSION = "3.2"
    }
  }
	
  stage('Print Stage'){
    echo $VERSION
  }
}
