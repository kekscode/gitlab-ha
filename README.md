# Howto HA with Gitlab

This architecture is based on the monolithic images of GitLab which provides
all the processes inside a single container.

**Note:** This is usually an anti-pattern in docker world.

# Components and criticality

* A Docker installation on the host where the container runs
* GitLab application dependencies
  * gitaly*
  * gitlab-monitor*
  * gitlab-workhorse*
  * logrotate*
  * nginx*
  * node-exporter*
  * postgres-exporter*
  * postgresql*
  * prometheus*
  * redis*
  * redis-exporter*
  * sidekiq*
  * sshd*
  * unicorn*

# Strategy

## Failover scenarios

# System design

[1]: https://docs.gitlab.com/omnibus/docker/#gitlab-docker-images
