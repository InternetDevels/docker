# Docker image with Jenkins and Docker.
More details about using Docker in Jenkins (how and why) see in [this article](http://container-solutions.com/running-docker-in-jenkins-in-docker/)

#### Usage
- Copy this directory to your server
- Docker and Docker compose should be installed. This [Ansible playbook](../../install-docker) can help.
- Run `docker-compose up -d`
- Your Jenkins installation will be available on `8080` port
- Now you can run Docker containers from jenkins jobs using `sudo`. Like:

    `sudo docker run -rm -v $(pwd):/app phpunit/phpunit ExampleTest.php`

