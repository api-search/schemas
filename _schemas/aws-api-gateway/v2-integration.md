---
description: Integration schema from Amazon API Gateway v2 API
layout: schema
name: Integration
properties_list:
- description: Integration identifier.
  name: IntegrationId
  type: string
- description: Type of integration (AWS_PROXY, HTTP_PROXY, etc.).
  name: IntegrationType
  type: string
- description: Integration target URI.
  name: IntegrationUri
  type: string
- description: Payload format version.
  name: PayloadFormatVersion
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-integration-schema.json
slug: v2-integration
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Integration
---
