# Windows IIS

Build and run the Docker image:

```bash
docker build -t iis-site .
docker run -d -p 8000:80 --name my-running-site iis-site
```

## Links

* [Windows IIS - Docker Hub](https://hub.docker.com/_/microsoft-windows-servercore-iis)
