# This is LabStack

This a stack that I'm using to provide miscellaneous services in a network lab.

This stack can be deployed using:
**`docker stack deploy -c docker-compose-swarm.yml LabStack`**

### What's included?

- Traefik v2.3 reverse proxy to route services into the swarm.

- An instance of **dnsmasq** that reads the `/etc/hosts` file of the host that
  it's running on to provide names to the lab.

- A Ghost blog. This is an instance of ghost labeled to run under the
  `/documentation` path. It's data is held in a Docker volume named
  `lab_documentation`.
