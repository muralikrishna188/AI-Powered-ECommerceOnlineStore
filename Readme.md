# 🛒 AI-Powered E-Commerce Online Store Microservices App on AKS + OpenAI

This project is a real-world, production-grade e-commerce application built using **10 microservices**, deployed on **Azure Kubernetes Service (AKS)**, and powered by **OpenAI** for intelligent customer interactions.

It replicates real-time enterprise architecture with scalable frontend/backend services, secure DevSecOps practices, real-time messaging, and AI-enhanced user experiences.

🧩 Frontend Microservices
StoreFront – Customer-facing e-commerce web UI

StoreAdmin – Admin dashboard for managing products/orders

🖥️ Backend Microservices
PlaceOrder – Handles order placement logic

Product – Manages product catalog and inventory

OrderProcessing – Manages order workflows and processing

🤖 AI Integration
AzureOpenAI – Connects to OpenAI APIs for chatbot, recommendations, and intelligent customer interactions

📬 Data & Messaging Services
OrderQueue (RabbitMQ) – Message broker for order events and asynchronous processing

OrderDB (MongoDB) – Stores order and customer transaction data

👥 Virtual Simulation
VirtualCustomer – Simulated customer service to test frontend and backend

VirtualWorker – Background service that consumes queue messages and processes orders

## 🔧 Tech Stack

- ⚙️ **Microservices:** StoreFront, StoreAdmin, PlaceOrder, Product, OrderProcessing, AzureOpenAI, OrderQueue (RabbitMQ), OrderDB (MongoDB), VirtualCustomer, VirtualWorker
- ☁️ **Cloud Platform:** Azure Kubernetes Service (AKS)
- 🧠 **AI Integration:** OpenAI GPT APIs (product description)
- 📊 **Observability:** Azure Monitor, App Insights, Grafana (optional)
- 🔄 **Messaging/Data:** RabbitMQ , Mongo DB

## MyOnline Store
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

