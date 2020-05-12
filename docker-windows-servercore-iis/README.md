# Windows Server Core Docker Image and IIS

Build and run the Docker image:

```bash
docker build -t servercore-iis .
docker run -it -p 8001:80 --name my-running-servercore-iis servercore-iis
```

## Links

* [Windows Server Core - Docker Hub](https://hub.docker.com/_/microsoft-windows-servercore)
