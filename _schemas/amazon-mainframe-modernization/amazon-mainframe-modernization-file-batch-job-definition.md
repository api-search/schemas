---
description: A file containing a batch job definition.
layout: schema
name: FileBatchJobDefinition
properties_list:
- description: ''
  name: fileName
  type: object
- description: ''
  name: folderPath
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-file-batch-job-definition-schema.json
slug: amazon-mainframe-modernization-file-batch-job-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-file-batch-job-definition-schema.json\",\n  \"title\": \"FileBatchJobDefinition\",\n  \"description\": \"A file containing a batch job definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the file containing the batch job definition.\"\n        }\n      ]\n    },\n    \"folderPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The path to the file containing the batch job definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-file-batch-job-definition-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: FileBatchJobDefinition
---
