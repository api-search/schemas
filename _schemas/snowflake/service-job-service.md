---
description: A Snowflake job service object.
layout: schema
name: JobService
properties_list:
- description: The current status of the service.
  name: status
  type: string
- description: Specifies the name of the compute pool in your account on which to run the service.
  name: compute_pool
  type: string
- description: Specifies the names of the external access integrations that allow your service to access external sites.
  name: external_access_integrations
  type: array
- description: Specifies a comment for the service.
  name: comment
  type: string
- description: True if the service is an async job service; false otherwise.
  name: is_async_job
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-job-service-schema.json
slug: service-job-service
source_filename: service-job-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobService\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake job service object.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the service.\"\n    },\n    \"compute_pool\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name of the compute pool in your account on which to run the service.\"\n    },\n    \"external_access_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the names of the external access integrations that allow your service to access external sites.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the service.\"\n    },\n    \"is_async_job\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the service is an async job service; false otherwise.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-job-service-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: JobService
---
