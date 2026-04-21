---
description: Route schema from Amazon API Gateway v2 API
layout: schema
name: Route
properties_list:
- description: Route identifier.
  name: RouteId
  type: string
- description: Route key (e.g. "GET /items" or "$connect").
  name: RouteKey
  type: string
- description: Integration target reference.
  name: Target
  type: string
- description: Authorization type for the route.
  name: AuthorizationType
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-route-schema.json
slug: v2-route
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Route
---
