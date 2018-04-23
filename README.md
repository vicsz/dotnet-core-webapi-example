# dotnet-core-webapi-example - Setup Steps from scratch

## Install NET Core SDK

## Create a new Web API project 

_#dotnet new webapi -o dotnet-core-webapi-example_

## Run the App From the dotnet-core-webapi-example directory : 

_#cd dotnet-core-webapi-example_

_#dotnet run

## Verify Application is running by making a call to it :

_#curl localhost:5000/api/values_

## Install Cloud Foundry commandline 

_#brew tap cloudfoundry/tap_

_#brew install cf-cli_

## Connect and login to your PCF instance (you can try a trial one at (https://run.pivotal.io)

_#cf login -a add.pcf.api.url.here_

## Create a PCF space (if needed)

_#cf create-space sample-space_

## Build your app 

_#cf dotnet publish_

## Deploy app to PCF 

_#cf push dotnet-core -p bin/Debug/netcoreapp2.0/_  (where dotnetcore will be your PCF app name)




