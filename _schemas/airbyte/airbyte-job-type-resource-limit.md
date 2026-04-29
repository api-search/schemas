---
description: sets resource requirements for a specific job type for an actor or actor definition. these values override the default, if both are set.
layout: schema
name: JobTypeResourceLimit
properties_list:
- description: ''
  name: jobType
  type: object
- description: ''
  name: resourceRequirements
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-job-type-resource-limit-schema.json
slug: airbyte-job-type-resource-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-type-resource-limit-schema.json\",\n  \"title\": \"JobTypeResourceLimit\",\n  \"description\": \"sets resource requirements for a specific job type for an actor or actor definition. these values override the default, if both are set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobType\": {\n      \"$ref\": \"#/components/schemas/JobType\"\n    },\n    \"resourceRequirements\": {\n      \"$ref\": \"#/components/schemas/ResourceRequirements\"\n    }\n  },\n  \"required\": [\n    \"jobType\",\n    \"resourceRequirements\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-type-resource-limit-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: JobTypeResourceLimit
---
