---
description: ApiKey schema from Amazon API Gateway v1 API
layout: schema
name: ApiKey
properties_list:
- description: ApiKey identifier.
  name: id
  type: string
- description: Value of the ApiKey.
  name: value
  type: string
- description: Name of the ApiKey.
  name: name
  type: string
- description: Whether the ApiKey is enabled.
  name: enabled
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-api-key-schema.json
slug: v1-api-key
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: ApiKey
---
