---
description: ''
layout: schema
name: CreateConnectionRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: databaseType
  type: string
- description: ''
  name: host
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: serviceName
  type: string
- description: ''
  name: schema
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: agentHost
  type: string
- description: ''
  name: agentPort
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-create-connection-request-schema.json
slug: oracle-goldengate-veridata-rest-create-connection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateConnectionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"databaseType\": {\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"agentHost\": {\n      \"type\": \"string\"\n    },\n    \"agentPort\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-create-connection-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateConnectionRequest
---
