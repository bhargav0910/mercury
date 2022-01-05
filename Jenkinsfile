#!/usr/bin/env groovy

def VERSION
pipeline {

  agent none

  stages {
    stage('Init Stage') {
       VERSION = "3.2"
    }
	
    stage('Print Stage'){
      echo $VERSION
    }
  }
}

