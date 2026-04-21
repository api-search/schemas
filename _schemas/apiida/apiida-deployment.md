---
description: An API deployment operation that provisions a specific API version to one or more managed gateways.
layout: schema
name: APIIDA Deployment
properties_list:
- description: Unique deployment identifier
  name: id
  type: string
- description: Identifier of the API being deployed
  name: apiId
  type: string
- description: Version of the API being deployed
  name: version
  type: string
- description: List of target gateway identifiers
  name: targetGateways
  type: array
- description: Current status of the deployment
  name: status
  type: string
- description: Timestamp when the deployment was initiated
  name: createdAt
  type: string
- description: Timestamp when the deployment completed or failed
  name: completedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-deployment.json
slug: apiida-deployment
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA Deployment
---
