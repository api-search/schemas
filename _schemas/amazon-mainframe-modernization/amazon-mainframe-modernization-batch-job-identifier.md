---
description: Identifies a specific batch job.
layout: schema
name: BatchJobIdentifier
properties_list:
- description: ''
  name: fileBatchJobIdentifier
  type: object
- description: ''
  name: scriptBatchJobIdentifier
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-batch-job-identifier-schema.json
slug: amazon-mainframe-modernization-batch-job-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-identifier-schema.json\",\n  \"title\": \"BatchJobIdentifier\",\n  \"description\": \"Identifies a specific batch job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileBatchJobIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileBatchJobIdentifier\"\n        },\n        {\n          \"description\": \"Specifies a file associated with a specific batch job.\"\n        }\n      ]\n    },\n    \"scriptBatchJobIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptBatchJobIdentifier\"\n        },\n        {\n          \"description\": \"A batch job identifier in which the batch job to run is identified by the script name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-job-identifier-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: BatchJobIdentifier
---
