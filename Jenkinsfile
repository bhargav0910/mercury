pipeline {
    agent any
    environment {
        ENV_NAME = "${env.BRANCH_NAME}"
    }

    stages {
        stage('Build Container') {
            steps {
                echo 'Building Container..'
                echo 'Building Branch: ' + env.BRANCH_NAME
                echo 'Build Number: ' + env.BUILD_NUMBER
                echo 'Building Environment: ' + ENV_NAME

                echo "Running your service with environemnt ${ENV_NAME} now"
            }
        }
    }
}
