# PowerShell Docker Image

Build and run the Docker image:

```bash
docker build -t pwsh .
docker run -it --name my-running-powershell pwsh
```

## How to Use Windows Server Core Image

```bash
docker pull mcr.microsoft.com/powershell:latest
```

or

```bash
docker pull mcr.microsoft.com/powershell:preview
```

## Links

* [PowerShell - Docker Hub](https://hub.docker.com/_/microsoft-powershell)
