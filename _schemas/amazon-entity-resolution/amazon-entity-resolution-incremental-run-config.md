---
description: An object which defines an incremental run type and has only <code>incrementalRunType</code> as a field.
layout: schema
name: IncrementalRunConfig
properties_list:
- description: ''
  name: incrementalRunType
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-incremental-run-config-schema.json
slug: amazon-entity-resolution-incremental-run-config
source_filename: amazon-entity-resolution-incremental-run-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-incremental-run-config-schema.json\",\n  \"title\": \"IncrementalRunConfig\",\n  \"description\": \"An object which defines an incremental run type and has only <code>incrementalRunType</code> as a field.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incrementalRunType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncrementalRunType\"\n        },\n        {\n          \"description\": \"The type of incremental run. It takes only one value: <code>IMMEDIATE</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-incremental-run-config-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: IncrementalRunConfig
---
