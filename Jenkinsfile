pipeline {
    agent any
    environment {
        REVISION = ""
    }
    stages {
        stage('Example') {
            steps {
                script{
                    my_var = 'value1'
		    my_var1 = 'hello'
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
