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
source_filename: management-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the client connected.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"LastActiveAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent activity on the connection.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"Identity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"SourceIp\": {\n          \"type\": \"string\",\n          \"description\": \"Source IP address of the client.\",\n          \"example\": \"example-value\"\n        },\n        \"UserAgent\": {\n          \"type\": \"string\",\n          \"description\": \"User agent string from the client.\",\n          \"example\": \"example-value\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/management-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Connection schema from Amazon API Gateway management API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/management-connection-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Connection
---
