---
description: An environment in an Apigee organization. Environments provide a runtime execution context for API proxies, with separate settings for caches, target servers, keystores, and more.
layout: schema
name: Apigee Environment
properties_list:
- description: Required. Name of the environment.
  name: name
  type: string
- description: Display name for the environment.
  name: displayName
  type: string
- description: Description of the environment.
  name: description
  type: string
- description: Output only. State of the environment.
  name: state
  type: string
- description: Output only. Creation time in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Last modification time.
  name: lastModifiedAt
  type: string
- description: Deployment type of the environment.
  name: deploymentType
  type: string
- description: Type of API proxies deployed in this environment.
  name: apiProxyType
  type: string
- description: A collection of key-value property pairs.
  name: properties
  type: object
- description: Runtime node configuration for the environment.
  name: nodeConfig
  type: object
- description: Optional forward proxy URI for the environment.
  name: forwardProxyUri
  type: string
- description: Type of the environment.
  name: type
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-environment-schema.json
slug: apigee-environment
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
title: Apigee Environment
---
