---
description: Authorizer schema from Amazon API Gateway v2 API
layout: schema
name: Authorizer
properties_list:
- description: Authorizer identifier.
  name: AuthorizerId
  type: string
- description: Authorizer name.
  name: Name
  type: string
- description: Type of authorizer (REQUEST or JWT).
  name: AuthorizerType
  type: string
- description: Identity sources for the authorizer.
  name: IdentitySource
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-authorizer-schema.json
slug: v2-authorizer
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Authorizer
---
