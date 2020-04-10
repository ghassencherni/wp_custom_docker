node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        git https://github.com/ghassencherni/wp_custom_docker 
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        app = docker.build("registry.gitlab.com/ghassencherni/ghassen-devopstt")
    }

    stage('Test image') {
        /* Ideally, we would run a test framework against our image. */
     

        app.inside {
            sh 'echo "Tests passed"'
        }
    }

}
