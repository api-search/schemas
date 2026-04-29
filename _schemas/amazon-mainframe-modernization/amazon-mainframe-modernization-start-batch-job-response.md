---
description: StartBatchJobResponse schema from AWS Mainframe Modernization API
layout: schema
name: StartBatchJobResponse
properties_list:
- description: ''
  name: executionId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-start-batch-job-response-schema.json
slug: amazon-mainframe-modernization-start-batch-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-start-batch-job-response-schema.json\",\n  \"title\": \"StartBatchJobResponse\",\n  \"description\": \"StartBatchJobResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of this execution of the batch job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-start-batch-job-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: StartBatchJobResponse
---
