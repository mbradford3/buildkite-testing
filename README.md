# buildkite-testing
A repo created to test with buildkite

Worth noting that if you want the docker agents to run, you need to create a new pair of ssh keys on the Docker instance.

1) Login to the Docker container using the following commands:

- docker ps (to get the container id - in this case it was 7d...)

- docker exec -it 7d bash

2) Next run the following to add the new key pair:

- ssh-keygen -t rsa -b 4096

3) And output and copy the info:

- cat ~./ssh/id_rsa.pub


4) Go to GitHub settings and add the new id_rsa.pub key

