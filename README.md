# This is LabStack

This a stack that I'm using to provide miscellaneous services in a network lab.
Currently, those services are:

- A DNS resolver. This is intended to be an easy place to name hosts on the lab
  network. All hosts in the lab network can point to the IP of the host that is
  running the stack for easy resolution of local names. This is also intended
  as a recursive resolver for any hosts in the lab.

  The `docker-compose-swarm.yml` this stack can be deployed using
  `docker stack deploy --compose-file docker-compose-swarm.yml LabStack`
