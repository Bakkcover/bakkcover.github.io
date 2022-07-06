---
layout: default
title: Login
parent: User Authentication
nav_order: 1
---

# Login
{: .no_toc }

<details open markdown="block">
    <summary>
        Table of contents
    </summary>

- TOC
{:toc}

</details>

## Overview
An existing user will log in with:
* Username
* Password

## Implementation
When a user logs in, the username and password provided is authenticated with AWS Cognito.

If successful, a JWT token is returned and stored on Local Storage in the browser. 
This token is then subsequently sent in all future requests to access secured endpoints.