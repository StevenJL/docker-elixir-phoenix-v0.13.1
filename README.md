## Docker Image for Running Elixir 1.0.4 and Phoenix 0.13.1

This is based on [marcelocg/phoenix-docker](https://github.com/marcelocg/phoenix-docker) but runs Phoenix 0.13.1.

To use this image in your docker-ized phoenix app start your `Dockerfile` with this:

```
FROM hacker314159/docker-elixir-phoenix-v0.13.1
```

To just pull down this image from `hub.docker` and play around with it:
```shell
docker pull hacker314159/docker-elixir-phoenix-v0.13.1

docker images | grep phoenix
# hacker314159/docker-elixir-phoenix-v0.13.1   latest  12345abcdef

docker run -ti 12345abcdef /bin/bash
# to enter the docker container

iex -v
#=> Elixir 1.0.4

mix help | grep phoenix
#=> mix phoenix.new     # Create a new Phoenix v0.13.1 application
```


