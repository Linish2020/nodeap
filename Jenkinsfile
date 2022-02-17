node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'armor') {

        def customImage = docker.build("linish20/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}