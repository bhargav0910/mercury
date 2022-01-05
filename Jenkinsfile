node {
    def a
    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */
	 a = "This is a version test"

    }


    // code placeholder
    stage('Print message') {
      echo "${env.BUILD_NUMBER}"
      echo "$a"
    }
}
