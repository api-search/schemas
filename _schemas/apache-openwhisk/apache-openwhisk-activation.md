---
description: Activation schema from Apache OpenWhisk
layout: schema
name: Activation
properties_list:
- description: Unique activation identifier
  name: activationId
  type: string
- description: ''
  name: namespace
  type: string
- description: Name of invoked action/trigger
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: Subject who invoked the action
  name: subject
  type: string
- description: Start time epoch ms
  name: start
  type: integer
- description: End time epoch ms
  name: end
  type: integer
- description: Duration in milliseconds
  name: duration
  type: integer
- description: ''
  name: response
  type: object
- description: Activation log output
  name: logs
  type: array
- description: ''
  name: annotations
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-schema.json
slug: apache-openwhisk-activation
source_filename: apache-openwhisk-activation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-schema.json\",\n  \"title\": \"Activation\",\n  \"description\": \"Activation schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique activation identifier\",\n      \"example\": \"44794bd6aab74415b4e42a308d880727\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"guest\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of invoked action/trigger\",\n      \"example\": \"hello\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"0.0.1\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject who invoked the action\",\n      \"example\": \"\
  guest\"\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start time epoch ms\",\n      \"example\": 1718153645993\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"End time epoch ms\",\n      \"example\": 1718153646050\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in milliseconds\",\n      \"example\": 57\n    },\n    \"response\": {\n      \"$ref\": \"#/components/schemas/ActivationResponse\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Activation log output\"\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Activation
---
