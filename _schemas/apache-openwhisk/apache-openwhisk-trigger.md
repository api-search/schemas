---
description: Trigger schema from Apache OpenWhisk
layout: schema
name: Trigger
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: publish
  type: boolean
- description: ''
  name: annotations
  type: array
- description: ''
  name: parameters
  type: array
- description: ''
  name: updated
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-trigger-schema.json
slug: apache-openwhisk-trigger
source_filename: apache-openwhisk-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-trigger-schema.json\",\n  \"title\": \"Trigger\",\n  \"description\": \"Trigger schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"guest\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"myTrigger\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"0.0.1\"\n    },\n    \"publish\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"\
  updated\": {\n      \"type\": \"integer\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-trigger-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Trigger
---
