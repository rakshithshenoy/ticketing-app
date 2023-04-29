# Ticketing-App - Cloud Computing (UE20CS351)

This is an Ecommerce microservices project built with NextJS, Express with Typescript, NATS, Docker, Kubernetes and Github Actions. The purpose of this project is to create, manage and sell tickets online. The application consists of 5 backend microservices for creating tickets, orders, payments, expiration, and authentication.

## Installation

To install and run this application on your local machine, follow the steps below:

### Prerequisites

- Node.js (v14 or higher)
- Docker
- Kubernetes

### Steps

1. Clone the repository
2. Open the /etc/hosts file on Mac/ Linux and add `127.0.0.1 ticketing.dev` at the end of the file
3. cd into auth, client, expiration, orders, payments and tickets and run `npm install`
4. Install the ingress service by running `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.7.0/deploy/static/provider/cloud/deploy.yaml`
5. Stay at the root directory of this project and run `skaffold dev` in your terminal
6. Wait for all the pods to be up and running. All the microservices should show `Connected to mongo!`
7. Open your browser and navigate to `ticketing.dev`
8. If you get a warning saying that the page is not secure, you need to type `thisisunsafe` into browser and it'll take you to the webpage
