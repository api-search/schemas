---
description: Metadata about an API proxy in Apigee. API proxies act as facades for backend services, providing security, rate limiting, transformations, and other capabilities.
layout: schema
name: Apigee API Proxy
properties_list:
- description: Output only. Name of the API proxy.
  name: name
  type: string
- description: Output only. List of revisions defined for the API proxy.
  name: revision
  type: array
- description: Output only. The ID of the most recently created revision.
  name: latestRevisionId
  type: string
- description: ''
  name: metaData
  type: object
- description: User-defined labels for organizing API proxies.
  name: labels
  type: object
- description: Output only. Whether this proxy is read-only.
  name: readOnly
  type: boolean
- description: Type of the API proxy.
  name: apiProxyType
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-api-proxy-schema.json
slug: apigee-api-proxy
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
title: Apigee API Proxy
---
