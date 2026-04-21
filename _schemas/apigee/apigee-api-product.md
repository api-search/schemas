---
description: An API product bundles API resources (proxies) for consumption by developers. Products define access control, quotas, and which API proxies and resources are available.
layout: schema
name: Apigee API Product
properties_list:
- description: Internal name of the API product. Must be unique within the organization.
  name: name
  type: string
- description: Name displayed in the developer portal.
  name: displayName
  type: string
- description: Description of the API product.
  name: description
  type: string
- description: How API keys are approved for the product.
  name: approvalType
  type: string
- description: Custom attributes for the API product (maximum 18).
  name: attributes
  type: array
- description: Environments where this product is available.
  name: environments
  type: array
- description: API proxies included in this product.
  name: proxies
  type: array
- description: OAuth scopes associated with the product.
  name: scopes
  type: array
- description: Number of requests permitted per quota interval.
  name: quota
  type: string
- description: Time interval over which the quota is applied.
  name: quotaInterval
  type: string
- description: Time unit for the quota interval.
  name: quotaTimeUnit
  type: string
- description: ''
  name: operationGroup
  type: object
- description: Output only. Unix time when the product was created.
  name: createdAt
  type: string
- description: Output only. Unix time when the product was last modified.
  name: lastModifiedAt
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-api-product-schema.json
slug: apigee-api-product
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
title: Apigee API Product
---
