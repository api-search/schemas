---
description: Action schema from Apache OpenWhisk
layout: schema
name: Action
properties_list:
- description: Namespace owning the action
  name: namespace
  type: string
- description: Action name
  name: name
  type: string
- description: Action version
  name: version
  type: string
- description: Whether the action is public
  name: publish
  type: boolean
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
- description: Last update timestamp (epoch ms)
  name: updated
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-schema.json
slug: apache-openwhisk-action
source_filename: apache-openwhisk-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Action schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace owning the action\",\n      \"example\": \"guest\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Action name\",\n      \"example\": \"hello\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Action version\",\n      \"example\": \"0.0.1\"\n    },\n    \"publish\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the action is public\",\n      \"example\": false\n    },\n    \"exec\": {\n      \"$ref\": \"#/components/schemas/ActionExec\"\n    },\n    \"annotations\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"limits\": {\n      \"$ref\": \"#/components/schemas/ActionLimits\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Last update timestamp (epoch ms)\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Action
---
