---
description: RestApi schema from Amazon API Gateway v1 API
layout: schema
name: RestApi
properties_list:
- description: Identifier of the RestApi.
  name: id
  type: string
- description: Name of the RestApi.
  name: name
  type: string
- description: Description of the RestApi.
  name: description
  type: string
- description: Timestamp when the RestApi was created.
  name: createdDate
  type: string
- description: Version identifier of the API.
  name: version
  type: string
- description: ''
  name: endpointConfiguration
  type: object
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-rest-api-schema.json
slug: v1-rest-api
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: RestApi
---
