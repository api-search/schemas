---
description: Defines the details of a batch job.
layout: schema
name: BatchJobDefinition
properties_list:
- description: ''
  name: fileBatchJobDefinition
  type: object
- description: ''
  name: scriptBatchJobDefinition
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-batch-job-definition-schema.json
slug: amazon-mainframe-modernization-batch-job-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-definition-schema.json\",\n  \"title\": \"BatchJobDefinition\",\n  \"description\": \"Defines the details of a batch job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileBatchJobDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileBatchJobDefinition\"\n        },\n        {\n          \"description\": \"Specifies a file containing a batch job definition.\"\n        }\n      ]\n    },\n    \"scriptBatchJobDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptBatchJobDefinition\"\n        },\n        {\n          \"description\": \"A script containing a batch job definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-definition-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: BatchJobDefinition
---
