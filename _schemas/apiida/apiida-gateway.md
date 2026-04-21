---
description: A managed API gateway instance registered with APIIDA, typically a Broadcom Layer7 gateway used for API deployment and monitoring.
layout: schema
name: APIIDA Gateway
properties_list:
- description: Unique gateway identifier
  name: id
  type: string
- description: Display name of the gateway
  name: name
  type: string
- description: Hostname or IP address of the gateway
  name: host
  type: string
- description: Gateway management port
  name: port
  type: integer
- description: Current connection status of the gateway
  name: status
  type: string
- description: Gateway platform type (e.g. Layer7, Kong, AWS)
  name: type
  type: string
- description: Gateway software version
  name: version
  type: string
- description: Number of APIs currently deployed on this gateway
  name: apiCount
  type: integer
- description: Timestamp when the gateway was registered
  name: createdAt
  type: string
- description: Timestamp when the gateway record was last updated
  name: updatedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-gateway.json
slug: apiida-gateway
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA Gateway
---
