---
description: Represents a deployment of an API proxy revision to an environment in Apigee. Deployments make API proxies available to receive and process client requests.
layout: schema
name: Apigee Deployment
properties_list:
- description: Environment where the proxy is deployed.
  name: environment
  type: string
- description: API proxy name.
  name: apiProxy
  type: string
- description: API proxy revision number.
  name: revision
  type: string
- description: Time the deployment was initiated.
  name: deployStartTime
  type: string
- description: Current state of the deployment.
  name: state
  type: string
- description: Status reported by individual runtime pods.
  name: pods
  type: array
- description: Conflicts with other deployments sharing the same base path.
  name: routeConflicts
  type: array
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-deployment-schema.json
slug: apigee-deployment
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Deployment
---
