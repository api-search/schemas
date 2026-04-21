---
description: Resource schema from Amazon API Gateway v1 API
layout: schema
name: Resource
properties_list:
- description: Resource identifier.
  name: id
  type: string
- description: Parent resource identifier.
  name: parentId
  type: string
- description: Last path segment for this resource.
  name: pathPart
  type: string
- description: Full path of the resource.
  name: path
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-resource-schema.json
slug: v1-resource
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Resource
---
