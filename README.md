# About this Repo

This is the Git repo of the Docker image for [nginx-sticky](https://hub.docker.com/r/imkulikov/nginx-sticky/).

## About nginx build:

This is simple and slim image (**≈8mb**) with builtin [nginx-sticky-module-ng](https://bitbucket.org/nginx-goodies/nginx-sticky-module-ng/overview)

Nginx build with:
- http_realip_module
- http_addition_module
- http_sub_module
- http_gunzip_module
- http_gzip_static_module
- threads
- stream
- stream_realip_module
- compat
- nginx-sticky-module

## Why I build this container:

When I worked around nginx + pm2 (cluster) + nodejs + websockets,
faced with the problem that the nginx + pm2-cluster + websocket
is not working properly and I needed to implement some kind
of layer between the app's container and nginx.
The task of this layer is to provide sticky sessions

## License

[MIT License](License.md)