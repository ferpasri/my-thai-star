FROM microsoft/dotnet:latest
 
COPY . /app
WORKDIR /app/OASP4Net.Application.WebApi
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

ENV ASPNETCORE_URLS http://0.0.0.0:9082
EXPOSE 9082/tcp
ENTRYPOINT ["dotnet", "run"]