# Vector Search Demos

## Steps for getting it running

1. Run `azd up` on [azure-search-openai-demo](https://github.com/Azure-Samples/azure-search-openai-demo/) with GPT-4-vision enabled. This will create the necessary resources for the Azure OpenAI, Azure AI Search services, and the Computer Vision service.

2. Create a .env with these variables, and the values taken from `.azure/ENV-NAME/.env`

```shell
AZURE_OPENAI_SERVICE=YOUR-SERVICE-NAME
AZURE_OPENAI_DEPLOYMENT_NAME=YOUR-OPENAI-DEPLOYMENT-NAME
AZURE_OPENAI_ADA_DEPLOYMENT=YOUR-EMBED-DEPLOYMENT-NAME
AZURE_SEARCH_SERVICE=YOUR-SEARCH-SERVICE-NAME
AZURE_COMPUTERVISION_SERVICE=YOUR-COMPUTERVISION-SERVICE-NAME
```

3. Login to the Azure Developer CLI:

```shell
azd auth login
```