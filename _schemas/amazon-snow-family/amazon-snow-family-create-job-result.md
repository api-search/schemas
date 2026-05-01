---
description: CreateJobResult schema from Amazon Snow Family API
layout: schema
name: CreateJobResult
properties_list:
- description: ''
  name: JobId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-job-result-schema.json
slug: amazon-snow-family-create-job-result
source_filename: amazon-snow-family-create-job-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-job-result-schema.json\",\n  \"title\": \"CreateJobResult\",\n  \"description\": \"CreateJobResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a job, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-job-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateJobResult
---
