# Windows Server Core Docker Image

Build and run the Docker image:

```bash
docker build -t servercore .
docker run -it --name my-running-servercore servercore
```

## How to Use Windows Server Core Image

```bash
docker run mcr.microsoft.com/windows/servercore:ltsc2019
```

## Links

* [Windows Server Core - Docker Hub](https://hub.docker.com/_/microsoft-windows-servercore)
