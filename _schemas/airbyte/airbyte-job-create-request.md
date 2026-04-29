---
description: Creates a new Job from the configuration provided in the request body.
layout: schema
name: JobCreateRequest
properties_list:
- description: ''
  name: connectionId
  type: string
- description: ''
  name: jobType
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-job-create-request-schema.json
slug: airbyte-job-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-create-request-schema.json\",\n  \"title\": \"JobCreateRequest\",\n  \"description\": \"Creates a new Job from the configuration provided in the request body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"jobType\": {\n      \"$ref\": \"#/components/schemas/JobTypeEnum\"\n    }\n  },\n  \"required\": [\n    \"jobType\",\n    \"connectionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: JobCreateRequest
---
