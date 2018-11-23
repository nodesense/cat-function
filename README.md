# Get started


```

Ensure you have node.js 8.x LTS

npm install -g azure-functions-core-tools


ensure you update local.settings.json with your storage account connection string for the timer functions


local.settings.json

{
  "IsEncrypted": false,
  "Values": {
    "AzureWebJobsStorage": "DefaultEndpointsProtocol=https;AccountName=catstorageworkshop2;AccountKey=......;EndpointSuffix=core.windows.net",
    "FUNCTIONS_WORKER_RUNTIME": "java"
  }
}



git clone https://github.com/nodesense/cat-function

cd cat-function

mvn clean package 

open eclipse, import maven project

mvn azure-functions:run


az login


mvn azure-functions:deploy




```