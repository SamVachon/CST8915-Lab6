# CST8915 Lab 6 — Algonquin Pet Store on AKS

**Samuel Vachon**,
**041101891**

I deployed the Algonquin Pet Store to Azure Kubernetes Service (AKS) using the provided Kubernetes manifest. The application includes the storefront, Product Service, Order Service, and RabbitMQ.

## Demo

[Watch the Lab 6 demo on YouTube](https://www.youtube.com/watch?v=sowu9ongfkY)

## How the services share one public IP

The storefront's Kubernetes LoadBalancer Service provides a public IP. NGINX serves the web app and forwards requests based on their path. It sends `/products` to the Product Service, `POST /orders` to the Order Service, and `/rabbitmq/` to the RabbitMQ management dashboard.

[Lab instructions and deployment manifest](https://github.com/ramymohamed10/26F_CST8915_Lab6)
