 
 <img src="https://github.com/khanasif1/Simply-Dapr/img/dapr.png" alt="DAPR">
 <img src="https://github.com/khanasif1/Simply-Dapr/blob/7e2b703ccc84e6f977e50a8dd7afe7283d2fcd33/img/dapr-components.png" alt="DAPR">
# Simply-Dapr
This repository is a simple contains code and samples for Dapr

## Create a Web API Project
Install dotnet SDK
Run dotnet new  webapi --no-https --name <App Name>
## Install the Dapr CLI
The Dapr CLI is the main tool you’ll be using for various Dapr related tasks. You can use it to run an application with a Dapr sidecar, as well as review sidecar logs, list running services, and run the Dapr dashboard. 

## Run the init CLI command

Install the latest Dapr runtime binaries:

dapr init

## Verify containers are running
As mentioned above, the dapr init command launches several containers that will help you get started with Dapr. Verify this by running:

docker ps

## Run .net API using Dapr
dapr run --app-id dapr-pub-App --dapr-http-port 3500 --app-port 5000 dotnet run
