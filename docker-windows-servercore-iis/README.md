# Windows Server Core Docker Image and IIS

Build and run the Docker image:

```bash
docker build -t servercore-iis-site .
docker run -it -p 8001:80 servercore-iis-site
```

## Links

* [Windows Server Core - Docker Hub](https://hub.docker.com/_/microsoft-windows-servercore)
