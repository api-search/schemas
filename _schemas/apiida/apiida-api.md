---
description: An API managed within the APIIDA API Control Plane, representing a logical API resource that can be versioned and deployed to gateways.
layout: schema
name: APIIDA API
properties_list:
- description: Unique identifier for the API
  name: id
  type: string
- description: Display name of the API
  name: name
  type: string
- description: Human-readable description of the API
  name: description
  type: string
- description: Current lifecycle status of the API
  name: status
  type: string
- description: Tags for categorizing the API
  name: tags
  type: array
- description: The current active version identifier
  name: currentVersion
  type: string
- description: Timestamp when the API was created
  name: createdAt
  type: string
- description: Timestamp when the API was last updated
  name: updatedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-api.json
slug: apiida-api
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA API
---
