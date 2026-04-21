---
description: Api schema from Amazon API Gateway v2 API
layout: schema
name: Api
properties_list:
- description: Identifier of the API.
  name: ApiId
  type: string
- description: Name of the API.
  name: Name
  type: string
- description: API protocol (HTTP or WEBSOCKET).
  name: ProtocolType
  type: string
- description: Default endpoint for the API.
  name: ApiEndpoint
  type: string
- description: Route selection expression for the API.
  name: RouteSelectionExpression
  type: string
- description: Timestamp when the API was created.
  name: CreatedDate
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-api-schema.json
slug: v2-api
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Api
---
