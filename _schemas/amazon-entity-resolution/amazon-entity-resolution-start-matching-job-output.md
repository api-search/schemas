---
description: StartMatchingJobOutput schema from AWS EntityResolution
layout: schema
name: StartMatchingJobOutput
properties_list:
- description: ''
  name: jobId
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-start-matching-job-output-schema.json
slug: amazon-entity-resolution-start-matching-job-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-start-matching-job-output-schema.json\",\n  \"title\": \"StartMatchingJobOutput\",\n  \"description\": \"StartMatchingJobOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The ID of the job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-start-matching-job-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: StartMatchingJobOutput
---
