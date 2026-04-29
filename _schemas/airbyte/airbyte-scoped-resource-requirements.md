---
description: actor or actor definition specific resource requirements. if default is set, these are the requirements that should be set for ALL jobs run for this actor definition. it is overriden by the job type specific configurations. if not set, the platform will use defaults. these values will be overriden by configuration at the connection level.
layout: schema
name: ScopedResourceRequirements
properties_list:
- description: ''
  name: default
  type: object
- description: ''
  name: jobSpecific
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-scoped-resource-requirements-schema.json
slug: airbyte-scoped-resource-requirements
source_filename: airbyte-scoped-resource-requirements-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-scoped-resource-requirements-schema.json\",\n  \"title\": \"ScopedResourceRequirements\",\n  \"description\": \"actor or actor definition specific resource requirements. if default is set, these are the requirements that should be set for ALL jobs run for this actor definition. it is overriden by the job type specific configurations. if not set, the platform will use defaults. these values will be overriden by configuration at the connection level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"$ref\": \"#/components/schemas/ResourceRequirements\"\n    },\n    \"jobSpecific\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobTypeResourceLimit\"\n      }\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-scoped-resource-requirements-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ScopedResourceRequirements
---
