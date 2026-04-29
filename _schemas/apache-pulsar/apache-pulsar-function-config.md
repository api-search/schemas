---
description: FunctionConfig schema from Apache Pulsar
layout: schema
name: FunctionConfig
properties_list:
- description: ''
  name: tenant
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: className
  type: string
- description: ''
  name: inputs
  type: array
- description: ''
  name: output
  type: string
- description: ''
  name: logTopic
  type: string
- description: ''
  name: processingGuarantees
  type: string
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: runtime
  type: string
- description: ''
  name: autoAck
  type: boolean
- description: ''
  name: userConfig
  type: object
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-function-config-schema.json
slug: apache-pulsar-function-config
source_filename: apache-pulsar-function-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-function-config-schema.json\",\n  \"title\": \"FunctionConfig\",\n  \"description\": \"FunctionConfig schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"className\": {\n      \"type\": \"string\"\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"output\": {\n      \"type\": \"string\"\n    },\n    \"logTopic\": {\n      \"type\": \"string\"\n    },\n    \"processingGuarantees\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ATLEAST_ONCE\",\n        \"ATMOST_ONCE\",\n        \"EFFECTIVELY_ONCE\"\n      ]\n\
  \    },\n    \"parallelism\": {\n      \"type\": \"integer\"\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"JAVA\",\n        \"PYTHON\",\n        \"GO\"\n      ]\n    },\n    \"autoAck\": {\n      \"type\": \"boolean\"\n    },\n    \"userConfig\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-function-config-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: FunctionConfig
---
