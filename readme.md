# mstack Teamspeak Server
[![Build Status](https://travis-ci.com/mstackio/image-teamspeak.svg?branch=main)](https://travis-ci.com/mstackio/image-teamspeak)
![GitHub](https://img.shields.io/github/license/mstackio/image-teamspeak)
![Docker Pulls](https://img.shields.io/docker/pulls/mstackio/teamspeak)

This docker image allows you to run a Teamspeak server. This image is built on Alpine Linux and is about 37 MB with TS3.


Example usage (no persistent storage; for testing only - you will lose your data when the container is removed):

```
docker run -d --name teamspeak \
  -e TS3SERVER_LICENSE=accept \
  -p 9987:9987/udp -p 30033:30033 -p 10011:10011 -p 41144:41144 \
  mstackio/teamspeak
```

---

A project by [![Mstack](https://avatars3.githubusercontent.com/u/61955974?s=42&v=4)](https://mstack.io/)

