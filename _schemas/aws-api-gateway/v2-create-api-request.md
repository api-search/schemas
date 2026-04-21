---
description: CreateApiRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateApiRequest
properties_list:
- description: Name of the API.
  name: Name
  type: string
- description: Protocol type for the API.
  name: ProtocolType
  type: string
- description: Route selection expression (required for WebSocket APIs).
  name: RouteSelectionExpression
  type: string
- description: Description of the API.
  name: Description
  type: string
- description: Quick-create target Lambda or HTTP endpoint URI.
  name: Target
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-api-request-schema.json
slug: v2-create-api-request
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateApiRequest
---
