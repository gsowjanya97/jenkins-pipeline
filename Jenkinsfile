pipeline{
    agent any

    stages {
        stage("Build") {
            steps {
                sh '''sudo docker image build -t ubuntu:flask .
                sudo docker run -d --hostname webserv1 --name webserv1 -p 80:5000 ubuntu:flask
                sudo docker exec webserv1 ps'''
            }
        }

        stage("Test") {
            steps {
                sh 'curl -v localhost'
                
            }
        }
    }
}