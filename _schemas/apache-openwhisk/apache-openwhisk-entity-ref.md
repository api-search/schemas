---
description: EntityRef schema from Apache OpenWhisk
layout: schema
name: EntityRef
properties_list:
- description: Entity name
  name: name
  type: string
- description: ''
  name: annotations
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-entity-ref-schema.json
slug: apache-openwhisk-entity-ref
source_filename: apache-openwhisk-entity-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-entity-ref-schema.json\",\n  \"title\": \"EntityRef\",\n  \"description\": \"EntityRef schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Entity name\",\n      \"example\": \"hello\"\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-entity-ref-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: EntityRef
---
