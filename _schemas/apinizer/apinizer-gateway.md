---
description: Schema representing an API gateway managed by the Apinizer platform
layout: schema
name: Apinizer Gateway
properties_list:
- description: Unique identifier of the gateway
  name: id
  type: string
- description: Name of the gateway
  name: name
  type: string
- description: Description of the gateway
  name: description
  type: string
- description: Base URL of the backend service
  name: baseUrl
  type: string
- description: Gateway status
  name: status
  type: string
- description: Creation timestamp
  name: createdAt
  type: string
provider_name: Apinizer
provider_slug: apinizer
schema_file: json-schema/apinizer-gateway-schema.json
slug: apinizer-gateway
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
title: Apinizer Gateway
---
