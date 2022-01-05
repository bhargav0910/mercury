def  browser = 'Unknown'

pipeline {
    agent any
    stages {
        stage('SNAPSHOT') {
            steps {
                echo "SNAPSHOT"
                browser = "firefox"
                }
            }
        stage('RELEASE') {
             steps {
                echo "${browser}"
                }
            }
    }//end of stages 
}//end of pipeline
