pipeline {
    agent any
    environment {
        VERSION = "3.2"
    }
    stages {
        stage('Build Container') {
            steps {
              echo 'Building Container..'
            }
	}

	stage('Print'){
	  steps{
            echo $VERSION
	  }
	}
    }
}
