node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        app = docker.build("getintodevops/hellonode")
    }


    // code placeholder
    stage('Print message') {
       /* Finally, we'll push the image with two tags:
        * First, the incremental build number from Jenkins
        * Second, the 'latest' tag. */
       // withCredentials([usernamePassword( credentialsId: 'docker-hub-credentials', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {

        //  docker.withRegistry('localhost:5000', 'docker-hub-credentials') {
       //       sh "docker login -u bhargav1997 -p Teja@123"
         //      app.push("${env.BUILD_NUMBER}")
           //    app.push("latest")

	   echo "${env.BUILD_NUMBER}"
	   echo "Hi"
	
  }
    stage('helm update'){
      steps{
        container('build'){
          sh """
            cd /tmp
            rm -rf pyhton
            git clone https://github.com/bhargav0910/pyhton.git
            sed -i 's/^version: .*/version: '"2.500"'/' /tmp/pyhton/bhargav/Chart.yaml
            helm package --app-Version 2.500 /tmp/pyhton/bhargav/
         """
       }
     }
   }
}
