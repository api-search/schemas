---
description: ''
layout: schema
name: Service
properties_list:
- description: Service name
  name: name
  type: string
- description: Service type
  name: type
  type: string
- description: Service status
  name: status
  type: string
- description: Service listening port
  name: port
  type: integer
- description: Whether the service uses SSL/TLS
  name: secure
  type: boolean
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-service-schema.json
slug: oracle-goldengate-rest-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Service type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Service status\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Service listening port\"\n    },\n    \"secure\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the service uses SSL/TLS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-service-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Service
---
