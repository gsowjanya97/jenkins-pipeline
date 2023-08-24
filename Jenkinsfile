pipeline{
    agent any

    stages {
        stage("Build") {
            steps {
                docker image build -t ubuntu:flask .
                docker run -d --hostname webserv1 --name webserv1 -p 80:5000 ubuntu:flask
                docker exec webserv1 ps
            }
        }

        stage("Test") {
            curl localhost
        }
    }
}