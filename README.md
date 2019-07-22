Docker RSS
=========

a rss server use docker.

Deploy
------

1. put the `docker_rss.yml` to your server.

2. create directory `/home/username/docker/tts` to store rss data.

3. run command as below:

```
docker swarm init
docker stack deploy -c docker_rss.yml docker_rss
```

4. visit `http://localhost:8080` and config rss.

>you may need to manually pull these image from the docker hub.

Shutdown
--------

```
docker stack rm docker_rss
```

Dependents
----------

- [Tiny Tiny RSS](https://tt-rss.org/): a free and open source web-based news feed (RSS/Atom) reader and aggregator
- [RSS Hub](https://github.com/DIYgod/RSSHub): 一个轻量、易于扩展的 RSS 生成器，可以给任何奇奇怪怪的内容生成 RSS 订阅源。