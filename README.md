webapi using clean architecture with CQRS

## Create migrations

inside the solution folder

```shell
dotnet-ef migrations add <migration_name> -p src/Infra/Infra.csproj -s src/Core/Core.csproj
```

## Update database

inside the solution folder

```shell
dotnet-ef database update -p src/Infra/Infra.csproj -s src/Core/Core.csproj
```

## Run project

```shell
cd src/Core

dotnet run
```