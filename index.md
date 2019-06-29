---
layout: default
title: Home
nav_order: 1
description: "SaaSBox is a NodeJS / ExpressJS based template for building a software as a service SaaS business."
permalink: /
---

# SaaSBox Getting Started
{: .fs-9 }

SaaSBox is a SaaS template for Node / ExpressJS. It is an accelerated starting point for building a Software-as-a-service (SaaS) with a few crucial pages (landing, feature, pricing, products) editable with forms, creation and syncing of Stripe plans, sign up via email and social networks using PassportJS.
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Buy the Template](https://saasbox.net/products){: .btn .fs-5 .mb-4 .mb-md-0 }
---

## Prerequisites
Familiarity with NodeJS / ExpressJS, javascript.

If you are new to NodeJS, check out this free and high quality NodeJS SaaS / Web Application building [video crash course](https://getbuzz.io/c/learning-expressjs). Learn how to install NodeJS, create an MVC application with ExpressJS, make basic SQL queries with Sequelize, how to create a migration, a basic CRUD implementation and more. SaaSBox is in fact based on an advancement of this tutorial.

## Getting started

### Download

You can buy and download the template at this [link](https://saasbox.net/products).

### Quick start:

Install all the dependencies:
```bash
npm install
```

Run the migrations:

```bash
sequelize db:migrate
```

Create and edit a `.env` file in the root directory:

```bash
touch .env
sublime .env
```

Create Environment variables as below:
```bash
NODE_ENV=development
cf_privateKeyPath=
cf_accessKeyId=

s3_iam_user=
s3_accessKey=
s3_secret=

stripe_privateKey_test=
stripe_privateKey_prod=
stripe_publicKey_test=
stripe_publicKey_prod=
twitter_consumerKey=
twitter_consumerSecret=
twitter_dev_callbackURL=http://127.0.0.1:8081/signup/twitter/return
twitter_prod_callbackURL=https://getbuzz.io/signup/twitter/return

google_clientID=
google_clientSecret=
google_dev_callbackURL=http://127.0.0.1:8081/o/oauth/google
google_prod_callbackURL=https://getbuzz.io/o/oauth/google

facebook_appId=
facebook_appSecret=
facebook_dev_callbackURL=http://127.0.0.1:8081/o/oauth/facebook
facebook_prod_callbackURL=https://getbuzz.io/o/oauth/facebook

backend=
```
### Run the local application:
```bash
DEBUG=myapp:* npm start
```

### Test your local instance

Fire up your browser and go to: `https://localhost:8081`

### Create admin user

Your first sign up becomes the admin user, so save your email and password you used.

### Hosting Options

Check out SaaSBox [plans](https://saasbox.net/pricing) for fully managed hosting options - this handles all hosting complexities and you only need a domain to start.

Hosting provides:
* PostgreSQL database (size depends on the plan),
* Load Balancer with NodeJS apps behind with auto-scaling, 
* An HTTPS certificate with auto-renew (you need to create a CNAME record to point at the server), 
* Secure file storage, in case you sell downloadable products
* CDN: Cloudfront configured to serve your public files, images etc.
* Automatic updates. E.g. we add a new SaaS feature: "Get product reviews from your users", this will get pushed and your SaaS migrated auto-updated.


---

## About the project

SaaSBox is a Buzz Software product. Find out more about tech entrepreneurship and building a SaaS at [https://getbuzz.io](https://getbuzz.io)

### License

Check the license at the root directory of your SaaSBox source code for details.
