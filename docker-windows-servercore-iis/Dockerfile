FROM mcr.microsoft.com/windows/servercore:ltsc2019

# Uses dism.exe to install the IIS role.
RUN dism.exe /online /enable-feature /all /featurename:iis-webserver /NoRestart

RUN powershell -NoProfile -Command Remove-Item -Recurse C:\inetpub\wwwroot\*
WORKDIR /inetpub/wwwroot
COPY html/ .

# Sets a command or process that will run each time a container is run from the new image
CMD [ "powershell" ]
