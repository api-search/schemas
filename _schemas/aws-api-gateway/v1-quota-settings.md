---
description: QuotaSettings schema from Amazon API Gateway v1 API
layout: schema
name: QuotaSettings
properties_list:
- description: Maximum number of requests in the period.
  name: limit
  type: integer
- description: Time period (DAY, WEEK, MONTH).
  name: period
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-quota-settings-schema.json
slug: v1-quota-settings
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: QuotaSettings
---
