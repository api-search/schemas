---
description: NamespaceEntities schema from Apache OpenWhisk
layout: schema
name: NamespaceEntities
properties_list:
- description: ''
  name: actions
  type: array
- description: ''
  name: triggers
  type: array
- description: ''
  name: rules
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-namespace-entities-schema.json
slug: apache-openwhisk-namespace-entities
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-namespace-entities-schema.json\",\n  \"title\": \"NamespaceEntities\",\n  \"description\": \"NamespaceEntities schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityRef\"\n      }\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityRef\"\n      }\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityRef\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-namespace-entities-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: NamespaceEntities
---
