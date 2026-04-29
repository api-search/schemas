---
description: ActionRequest schema from Apache OpenWhisk
layout: schema
name: ActionRequest
properties_list:
- description: ''
  name: exec
  type: object
- description: ''
  name: annotations
  type: array
- description: ''
  name: parameters
  type: array
- description: ''
  name: limits
  type: object
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-request-schema.json
slug: apache-openwhisk-action-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-request-schema.json\",\n  \"title\": \"ActionRequest\",\n  \"description\": \"ActionRequest schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exec\": {\n      \"$ref\": \"#/components/schemas/ActionExec\"\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"limits\": {\n      \"$ref\": \"#/components/schemas/ActionLimits\"\n    }\n  },\n  \"required\": [\n    \"exec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-request-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActionRequest
---
