---
description: A managed API gateway instance registered with APIIDA, typically a Broadcom Layer7 gateway used for API deployment and monitoring.
layout: schema
name: APIIDA Gateway
properties_list:
- description: Unique gateway identifier
  name: id
  type: string
- description: Display name of the gateway
  name: name
  type: string
- description: Hostname or IP address of the gateway
  name: host
  type: string
- description: Gateway management port
  name: port
  type: integer
- description: Current connection status of the gateway
  name: status
  type: string
- description: Gateway platform type (e.g. Layer7, Kong, AWS)
  name: type
  type: string
- description: Gateway software version
  name: version
  type: string
- description: Number of APIs currently deployed on this gateway
  name: apiCount
  type: integer
- description: Timestamp when the gateway was registered
  name: createdAt
  type: string
- description: Timestamp when the gateway record was last updated
  name: updatedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-gateway.json
slug: apiida-gateway
source_filename: apiida-gateway.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apiida-gateway.json\",\n  \"title\": \"APIIDA Gateway\",\n  \"description\": \"A managed API gateway instance registered with APIIDA, typically a Broadcom Layer7 gateway used for API deployment and monitoring.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"host\", \"port\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique gateway identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the gateway\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP address of the gateway\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Gateway management port\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"connected\", \"disconnected\", \"error\"],\n      \"description\": \"Current connection\
  \ status of the gateway\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Gateway platform type (e.g. Layer7, Kong, AWS)\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Gateway software version\"\n    },\n    \"apiCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of APIs currently deployed on this gateway\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the gateway was registered\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the gateway record was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/json-schema/apiida-gateway.json
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA Gateway
---
