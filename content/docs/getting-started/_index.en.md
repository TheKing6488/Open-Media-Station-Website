+++
title = 'Getting started'
+++

> **WARNING:** The software is in a very early stage of development. Please use it only for testing and not production.

## Server installation

1. At first get the Docker image for the server.

```sh
docker pull ghcr.io/openmediastation/openmediaserver:latest
```

2. Use the following environment variables.

```env
DOMAIN=example.com
AUTH_CLIENTID=AAAAAAAAAAAAAAAAAA
AUTH_CONFIGURATION_URL=https://auth.example.com/application/o/open-media-station/.well-known/openid-configuration
TMDB_KEY=aaaaaaaaaaaaaaaaaaaaaaa
```

3. Map the port `8080` of the container to your https port.

4. Make sure to mount your media directory to `/media` and provide a empty directory for the server files at `/config`.

## Get the clients

You can obtain the client from the artifacts of the latest [release](https://github.com/OpenMediaStation/OpenMediaStation.FE.MovieTV/releases).
