node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        /*checkout scm*/
        git 'https://github.com/miguelsd0501/hello-microservice'
    }

    stage('Compile package') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        /*app = docker.build("getintodevops/hellonode")*/
        sh 'mvn package'
    }
}
