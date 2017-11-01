Sometimes you want to command Docker on the host system from within a Docker container:

```
docker run -v /var/run/docker.sock:/var/run/docker.sock my-container
```
