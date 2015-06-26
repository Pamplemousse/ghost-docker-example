# Ghost in a Docker container

Using the [official image](https://github.com/docker-library/docs/tree/master/ghost).

```bash
docker pull ghost:latest
git clone git@github.com:Pamplemousse/ghost-docker-example.git
cd ghost-docker-example

docker run -d \
    --name 'ghost' \
    --publish 8002:2368 \
    --volume `pwd`/content:/var/lib/ghost \
    ghost
```

… connect to [http://localhost:8002](http://localhost:8001), et voilà!

 * user: **pony@double-rainbow.com**
 * password: **auieauie**
