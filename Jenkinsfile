node("windows") {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("mohamed99amine/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}