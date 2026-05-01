---
description: Identity schema from Amazon API Gateway management API
layout: schema
name: Identity
properties_list:
- description: Source IP address of the client.
  name: SourceIp
  type: string
- description: User agent string from the client.
  name: UserAgent
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/management-identity-schema.json
slug: management-identity
source_filename: management-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceIp\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the client.\",\n      \"example\": \"example-value\"\n    },\n    \"UserAgent\": {\n      \"type\": \"string\",\n      \"description\": \"User agent string from the client.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/management-identity-schema.json\",\n  \"title\": \"Identity\",\n  \"description\": \"Identity schema from Amazon API Gateway management API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/management-identity-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Identity
---
