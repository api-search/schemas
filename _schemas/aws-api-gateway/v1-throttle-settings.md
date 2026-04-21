---
description: ThrottleSettings schema from Amazon API Gateway v1 API
layout: schema
name: ThrottleSettings
properties_list:
- description: Burst limit for requests.
  name: burstLimit
  type: integer
- description: Steady-state rate limit (requests per second).
  name: rateLimit
  type: number
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-throttle-settings-schema.json
slug: v1-throttle-settings
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: ThrottleSettings
---
