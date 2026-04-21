---
description: Method schema from Amazon API Gateway v1 API
layout: schema
name: Method
properties_list:
- description: HTTP method verb.
  name: httpMethod
  type: string
- description: Authorization type for invoking the method.
  name: authorizationType
  type: string
- description: Whether the method requires an API key.
  name: apiKeyRequired
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-method-schema.json
slug: v1-method
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Method
---
