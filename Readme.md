
## Step by Step

## Frontend
StoreFront-Deployment.yml
StoreFront-LB-svc.yml

StoreAdmin-Deployment.yml
StoreAdmin-LB-svc.yml

## Backend
PlaceOrder-CLusterIP-SVC.yml
PlaceOrder-Deployment.yml

Product-Clusterip-svc.yml
Product-Deployment.yml

OrderProcessing-ClusterIP-svc.yml
OrderProcessing-Deployment.yml

# OpenAI
AzureOpenAI-ClutserIP-svc.yml
AzureOpenAI-Deployment.yml

# Data & Messaging
OrderQueue-RabbitMQ-Configmap.yml
OrderQueue-RabbitMQ-Statefulset.yml
OrderQueue-RabbitMQ-svc.yml

OrderDB-Mongo-Statefulset.yml
OrderDB-Mongo-svc.yml

# Virtual Customer & Worker
VirtualCustomer-Deployment.yml
VirtualWorker-Deployment.yml


## Steps:

1. Kubernetes CLuster
2. Azure Open AI

## 1. Setup Kubernetes CLuster
Subscription: Pay as you go
Resource group: EcommerceOnlineStoreRG
Kubernetes Cluster name: OnlinestoreKube005

az aks get-credentials -n OnlinestoreKube005 -g EcommerceOnlineStoreRG

Deploy Microservies

##2. Create Azure OpenAI

AZURE_OPENAI_DEPLOYMENT_NAME: gpt-4.1-mini
AZURE_OPENAI_ENDPOINT : ****
OPENAI_API_KEY : ***

Subscription: Pay as you go
Resourcegroup: OnlineStoreAIRG

