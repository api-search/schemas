---
description: ActionLimits schema from Apache OpenWhisk
layout: schema
name: ActionLimits
properties_list:
- description: Timeout in milliseconds
  name: timeout
  type: integer
- description: Memory in MB
  name: memory
  type: integer
- description: Log size limit in MB
  name: logs
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-limits-schema.json
slug: apache-openwhisk-action-limits
source_filename: apache-openwhisk-action-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-limits-schema.json\",\n  \"title\": \"ActionLimits\",\n  \"description\": \"ActionLimits schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in milliseconds\",\n      \"example\": 60000\n    },\n    \"memory\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory in MB\",\n      \"example\": 256\n    },\n    \"logs\": {\n      \"type\": \"integer\",\n      \"description\": \"Log size limit in MB\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-limits-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActionLimits
---
