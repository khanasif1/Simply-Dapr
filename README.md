# Dapr
This repository contains sample  code for Dapr
 
 <img src="https://github.com/khanasif1/Simply-Dapr/blob/7e2b703ccc84e6f977e50a8dd7afe7283d2fcd33/img/dapr.png" alt="DAPR" height="300">
 Dapr helps developers build event-driven, resilient distributed applications. Whether on-premises, in the cloud, or on an edge device, Dapr helps you tackle the challenges that come with building microservices and keeps your code platform agnostic.

 <img src="https://github.com/khanasif1/Simply-Dapr/blob/7e2b703ccc84e6f977e50a8dd7afe7283d2fcd33/img/dapr-components.png" alt="DAPR" height="300">

## Create a Web API Project
Install dotnet SDK
```console
Run dotnet new  webapi --no-https --name <App Name>
```

## Install the Dapr CLI
The Dapr CLI is the main tool you’ll be using for various Dapr related tasks. You can use it to run an application with a Dapr sidecar, as well as review sidecar logs, list running services, and run the Dapr dashboard. 

## Run the init CLI command

Install the latest Dapr runtime binaries:

```console
dapr init
```
## Verify containers are running
As mentioned above, the dapr init command launches several containers that will help you get started with Dapr. Verify this by running:

```console
docker ps
```
## Run .net API using Dapr

```console
dapr run --app-id dapr-pub-App --dapr-http-port 3500 --app-port 5000 dotnet run
```
