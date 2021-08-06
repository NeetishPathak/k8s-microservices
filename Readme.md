# Microservices Deployment using Kubernetes



![Architecture Diagram](./Microservices.png?raw=true "Architecture")

### Introduction 

In this project, five microservices will be deployed using kubernetes deployment and services.

1. Voting App : Voting App is a front end app written in python. This will be a user facing app that allows users to vote. This app should be run as  a deployment and a user facing service will allow access to the app.
>
2. Results App: Results App is also a front end app written in nodejs that would display live results. This app should be run as  a deployment and a user facing service will allow access to the interface.
>
3. Redis App: Redis App is a key value cache to save the vote registered from the Voting App. This app will be run as a deployment and a clusterIP service  will allow access to this service internally.
>
4. Postgres App: Postgres is the database that will store the votes. This app will be run as a deployment and a clusterIP service  will allow access to this service internally.
>
5. Worker App: The worker app will fetch votes from the redis and save it in postrgres


