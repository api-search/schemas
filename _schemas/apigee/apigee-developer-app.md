---
description: A developer app registered in Apigee. Apps are associated with developers and contain API keys (credentials) that provide access to API products.
layout: schema
name: Apigee Developer App
properties_list:
- description: Name of the developer app.
  name: name
  type: string
- description: Output only. ID of the developer app.
  name: appId
  type: string
- description: Output only. Developer ID of the owning developer.
  name: developerId
  type: string
- description: List of API products associated with the app.
  name: apiProducts
  type: array
- description: Custom attributes for the developer app.
  name: attributes
  type: array
- description: Callback URL used by OAuth 2.0 authorization servers.
  name: callbackUrl
  type: string
- description: Output only. Credentials (API keys) for the app.
  name: credentials
  type: array
- description: Status of the developer app.
  name: status
  type: string
- description: OAuth scopes associated with the app.
  name: scopes
  type: array
- description: Output only. Time the app was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the app was last modified.
  name: lastModifiedAt
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-developer-app-schema.json
slug: apigee-developer-app
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
title: Apigee Developer App
---
