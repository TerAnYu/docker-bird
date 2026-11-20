<h1 align="center">BIRD</h1>

<p align="center">The BIRD project aims to develop a fully functional dynamic IP routing daemon.</p>

<p align="center">
    <a href="https://ghcr.io/teranyu/bird">Container Registry</a> ·
    <a href="https://bird.network.cz">Project Source</a> ·
    <a href="https://bird.nic.cz/get-bird/">Download Latest</a>
</p>

<p align="center">
    <img src="https://img.shields.io/github/actions/workflow/status/TerAnYu/docker-bird/push.yml?branch=main" />
    <img src="https://img.shields.io/github/last-commit/TerAnYu/docker-bird" />
    <img src="https://img.shields.io/github/v/release/TerAnYu/docker-bird" />
    <img src="https://img.shields.io/github/release-date/TerAnYu/docker-bird" />
</p>

---

### Pull The Image

```bash
docker pull ghcr.io/teranyu/bird:latest
```

### Start Container

```bash
$ docker run -d \
  -v /etc/bird/:/etc/bird/ \
  --cap-add=NET_ADMIN \
  --cap-add=NET_BROADCAST \
  --cap-add=NET_RAW \
  --network=host \
  --restart=always \
  --name=bird \
  ghcr.io/teranyu/bird:latest
```
