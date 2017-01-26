# docker-nginx-ubuntu

An nginx Docker image based on ubuntu

## How it differes from the official nginx image?

The official image is based on Debian. The latest Debian 8 does not have the OpenSSL which supports ALPN.
Since Google Chrome browser dropped NPN support, HTTP/2 is no longer available if use the official image. 
Ubuntu Xenial (16.04) shipps OpenSSL 1.0.2 with ALPN support and fixes this problem.

## How to use?

```sh
docker pull lucidfrontier45/nginx
```