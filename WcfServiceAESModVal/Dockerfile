FROM microsoft/aspnet:4.6.2
ARG source
WORKDIR /inetpub/wwwroot
EXPOSE 5000/tcp
RUN ["aspnet", "restore"]
RUN ["aspnet","build"]
COPY ${source:-obj/Docker/publish} .
