
FROM  bitnami/aspnet-core:3.1



WORKDIR /app

# Copy the project files into the container
COPY *.csproj ./

RUN dotnet restore

COPY . .


RUN dotnet build -c Release


RUN dotnet publish -c Release -o /app/publish
EXPOSE 80
ENTRYPOINT ["dotnet", "run"]
