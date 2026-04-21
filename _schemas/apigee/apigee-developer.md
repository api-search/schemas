---
description: A developer registered in an Apigee organization. Developers are consumers of APIs who register apps and obtain API keys to access API products.
layout: schema
name: Apigee Developer
properties_list:
- description: Required. Email address of the developer. Used as the unique identifier.
  name: email
  type: string
- description: Required. First name of the developer.
  name: firstName
  type: string
- description: Required. Last name of the developer.
  name: lastName
  type: string
- description: Required. User name of the developer.
  name: userName
  type: string
- description: Output only. System-generated developer ID.
  name: developerId
  type: string
- description: Output only. Name of the Apigee organization.
  name: organizationName
  type: string
- description: Status of the developer account.
  name: status
  type: string
- description: Output only. List of apps owned by the developer.
  name: apps
  type: array
- description: Custom attributes for the developer (maximum 18).
  name: attributes
  type: array
- description: Output only. Companies associated with the developer.
  name: companies
  type: array
- description: Output only. Time the developer was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the developer was last modified in milliseconds since epoch.
  name: lastModifiedAt
  type: string
- description: Access type of the developer.
  name: accessType
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-developer-schema.json
slug: apigee-developer
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
title: Apigee Developer
---
