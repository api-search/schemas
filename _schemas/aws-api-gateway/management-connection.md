---
description: Connection schema from Amazon API Gateway management API
layout: schema
name: Connection
properties_list:
- description: Timestamp when the client connected.
  name: ConnectedAt
  type: string
- description: Timestamp of the most recent activity on the connection.
  name: LastActiveAt
  type: string
- description: ''
  name: Identity
  type: object
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/management-connection-schema.json
slug: management-connection
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Connection
---
