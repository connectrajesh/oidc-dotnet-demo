FROM mcr.microsoft.com/dotnet/sdk:6.0

WORKDIR /source

COPY *.csproj .
RUN ["dotnet", "restore"]

COPY . .
RUN ["dotnet", "build"]

EXPOSE 8080/tcp

ENTRYPOINT ["dotnet", "run"]
