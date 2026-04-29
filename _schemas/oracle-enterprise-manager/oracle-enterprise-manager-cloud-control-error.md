---
description: Error response returned by the API.
layout: schema
name: Error
properties_list:
- description: Machine-readable error code.
  name: errorCode
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: Additional details about the error.
  name: details
  type: string
- description: HTTP status code.
  name: httpStatusCode
  type: integer
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-error-schema.json
slug: oracle-enterprise-manager-cloud-control-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error response returned by the API.\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the error.\"\n    },\n    \"httpStatusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-error-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Error
---
