FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build-env
WORKDIR /app
COPY . ./
WORKDIR /app
COPY --from=build-env /app/out .
ENTRYPOINT ["dotnet","Api.dll"]
