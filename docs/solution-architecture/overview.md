---
layout: default
title: Overview
parent: Solution Architecture
nav_order: 1
---

# Overview
Bakkcover is hosted entirely on AWS infrastructure:
* An S3 bucket is used to host the frontend application as a static website.
  * The frontend application is built on Angular. 
* A single EC2 instance is used to host the backend application.
  * The backend application is built on the Spring Boot framework. 
* A single RDS instance is used to host a relational database.
  * PostgreSQL is used as the database.
* Cognito is used to for user authentication.
* Some Lambda functions are used to sync user information between Cognito and the RDS instance.
