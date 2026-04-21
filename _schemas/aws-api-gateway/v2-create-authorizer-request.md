---
description: CreateAuthorizerRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateAuthorizerRequest
properties_list:
- description: Name of the authorizer.
  name: Name
  type: string
- description: Type of authorizer.
  name: AuthorizerType
  type: string
- description: Identity sources to use.
  name: IdentitySource
  type: array
- description: URI of the Lambda authorizer (REQUEST type).
  name: AuthorizerUri
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-authorizer-request-schema.json
slug: v2-create-authorizer-request
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateAuthorizerRequest
---
