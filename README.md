# CAST AI - project for the Environment of Services Implementation AGH course.

## Topic

CAST AI - the leading all-in-one platform for Kubernetes automation, optimization, security, and cost management.

## Authors
- [Jakub Łubkowski](https://github.com/jakobcodes)
- [Kamil Miśkowiec](https://github.com/miskowieck)
- [Marcin Mikuła](https://github.com/mamikula)
- [Szymon Słota](https://github.com/sslota)

## Group 

Year: 2024
<br>
Group: nr. 5 - Thursday, 11:30 - 13:00

## 1. Introduction

[CAST AI](https://cast.ai/) is a cloud optimization platform that cuts cloud bills in half for AWS,
Google Cloud Platform, and Microsoft Azure customers who use the cloudnative technology of Kubernetes. Powered by AI, it analyzes multiple data
points to find an optimal cost-performance ratio.

### Goal of the project 

The aim of this project is to construct and perform a simple case study that would allow for familiarization with CAST.AI technology, which is an all-in-one platform for Kubernetes automation, optimization, security, and cost management.

## 2. Theoretical background/technology stack

CAST AI is an all-in-one platform for Kubernetes automation, optimization, security, and cost management. It abstracts layers of provider-specific technical complexity, so you can manage Kubernetes operations on all three major cloud providers with ease.

The platform comes with cost monitoring for real-time and longer-period cost reports at the cluster, namespace, and workload level. It also offers cost optimization suggestions and automatic optimization using autoscaling, spot instance automation, bin packing, and other features.

At the same time, CAST AI also checks your cluster security configuration for misconfigurations and any potential vulnerabilities and automatically prioritizes the fixes to improve your security posture. It also lets you scan your cluster against industry standards, incl. CIS Benchmarks and many more.

## 3. Case study concept description

In this case study, we will be using demo microservices provided by Google. The demo can be found at this link: https://github.com/GoogleCloudPlatform/microservices-demo. This set of demo microservices will be deployed on the AWS Cloud.
We will begin by setting up an environment on CAST AI for the microservices to run. Following this, we will deploy the microservices and monitor their performance, cost, and security using the tools provided by the CAST AI platform.

This hands-on experience will provide practical insights into the capabilities and benefits of using CAST AI for cloud optimization, Kubernetes automation, security enhancement, and cost management.

### Google microservices demo

**Online Boutique** is composed of 11 microservices written in different
languages that talk to each other over gRPC.

| Service                                              | Language      | Description                                                                                                                       |
| ---------------------------------------------------- | ------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| [frontend](/src/frontend)                           | Go            | Exposes an HTTP server to serve the website. Does not require signup/login and generates session IDs for all users automatically. |
| [cartservice](/src/cartservice)                     | C#            | Stores the items in the user's shopping cart in Redis and retrieves it.                                                           |
| [productcatalogservice](/src/productcatalogservice) | Go            | Provides the list of products from a JSON file and ability to search products and get individual products.                        |
| [currencyservice](/src/currencyservice)             | Node.js       | Converts one money amount to another currency. Uses real values fetched from European Central Bank. It's the highest QPS service. |
| [paymentservice](/src/paymentservice)               | Node.js       | Charges the given credit card info (mock) with the given amount and returns a transaction ID.                                     |
| [shippingservice](/src/shippingservice)             | Go            | Gives shipping cost estimates based on the shopping cart. Ships items to the given address (mock)                                 |
| [emailservice](/src/emailservice)                   | Python        | Sends users an order confirmation email (mock).                                                                                   |
| [checkoutservice](/src/checkoutservice)             | Go            | Retrieves user cart, prepares order and orchestrates the payment, shipping and the email notification.                            |
| [recommendationservice](/src/recommendationservice) | Python        | Recommends other products based on what's given in the cart.                                                                      |
| [adservice](/src/adservice)                         | Java          | Provides text ads based on given context words.                                                                                   |
| [loadgenerator](/src/loadgenerator)                 | Python/Locust | Continuously sends requests imitating realistic user shopping flows to the frontend.                                              |

## 4. Solution architecture

![image](https://github.com/mamikula/Environment-of-Services-Implementation/assets/85311656/52a2faa2-61a4-4a8c-95e4-163d1dee9504)

## 5. Environment configuration description

## 6. Installation method

## 7. How to reproduce - step by step

### Infrastructure as Code approach

## 8. Demo deployment steps:

### Configuration set-up

### Data preparation

### Execution procedure

### Results presentation

## 9. Summary – conclusions

## 10. References






