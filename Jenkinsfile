def my_var
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
                }
            }
        }

        stage('Example2') {
            steps {
                sh '''
                    echo ${my_var} 
                '''
            }
        }
    }
}
