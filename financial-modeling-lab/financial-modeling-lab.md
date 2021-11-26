# Financial Modelling in the Cloud

> Hands-on Lab

|                   |                       |
| :---------------- | :-------------------- |
| Proficiency Level | **Cloud  Enthusiast** |
| Tags              | ![https://img.shields.io/badge/%20-Financial%20Modeling-blue](https://img.shields.io/badge/%20-Financial%20Modeling-blue) |

## Lab Scenario

In this lab, you will estimate the cloud costs for the Task Management app that we designed in [Designing the REST API for a Task Management Application](../development-labs/api-development/task-management-api.design.md).

## What will you learn in this lab?

After completion of this lab, you will be able to:

- Understand what impacts the cloud costs of your application and what you can do to reduce that cost.

## Lab Instructions

### Exercise #1: Estimating the Costs for the Task Management Application

The objective of this lab is to estimate the costs of running the Task Management application using Microsoft Azure Services.

#### Utilized Azure Services

Here is the list of utilized Azure services and their purpose.

- Azure CDN to distribute the React-based web app that users can load in their browser to manage their tasks.
- Azure Active Directory for user authentication.
- Azure API Management for managing and protecting the Task Management APIs.
- Azure Managed Kubernetes (AKS) for running the Task Management API logic.
- Azure Cosmos DB to store user-profiles and task details.

#### Load Estimates

To estimate the resources, we need to have an idea of how many users will use the application and what traffic will they generate. We will not answer all those questions here but leave some for interpretation by you.

- We assume 10 million users who create on average five tasks per day.
- We assume that each user updates on average three tasks per day.
- We assume that the size of the React web app is 500KB and each user loads it at least once a day.
- We assume that 30% of the users load the app 3-5 times a day.

#### Things to Think About

Very often you will have only partial information like the one above that you can use to provide an estimate. It is OK to go back and research or ask for additional information. Here are few more things that you need to think of:

- What is the size of an average task request when a task is created? You will need to estimate this, but a good start will be to think of what the task fields are, how big they are (e., upper limits) and generate representative JSON from that. Then you need to take the file size of this JSON and increase it with some small number to account for the HTTP header information.
- You will need to also think of the growth of the data in Cosmos DB. Are you estimating for one year ahead, or for three years ahead, or for five years ahead? When the storage grows over time, the cost of maintaining the data will grow.
- If you assume the traffic, you need to make sure that this is submitted as a requirement to your IT and development teams. Let’s say you want to save money by compressing the outbound traffic – then, you will need to require your IT team to configure all web servers to use compression.
- Be careful with Azure API Management – it has a number of requests for the different tiers, and you need to make sure you choose the correct tier.

## Help improve this lab

[![Lab Issues](https://img.shields.io/github/issues/crimsonpinnacle/cloud-labs)](https://github.com/CrimsonPinnacle/cloud-labs/issues/new?assignees=toddysm&labels=new+lab&template=bug_template.md&title=) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/CrimsonPinnacle/cloud-labs/pulls)