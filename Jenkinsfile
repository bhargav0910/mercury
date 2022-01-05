pipeline {
    agent any
    environment {
        REVISION = ""
    }
    stages {
        stage('Example') {
            steps {
                script{
                    def my_var = 'value1'
		    def my_var1 = 'hello'
                }
            }
        }

        stage('Example2') {
            steps {
                sh """
		  echo "$my_var"
		  echo "$my_var1"
                """
            }
        }
    }
}
