---
description: A batch job identifier in which the batch job to run is identified by the file name and the relative path to the file name.
layout: schema
name: FileBatchJobIdentifier
properties_list:
- description: ''
  name: fileName
  type: object
- description: ''
  name: folderPath
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-file-batch-job-identifier-schema.json
slug: amazon-mainframe-modernization-file-batch-job-identifier
source_filename: amazon-mainframe-modernization-file-batch-job-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-file-batch-job-identifier-schema.json\",\n  \"title\": \"FileBatchJobIdentifier\",\n  \"description\": \"A batch job identifier in which the batch job to run is identified by the file name and the relative path to the file name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The file name for the batch job identifier.\"\n        }\n      ]\n    },\n    \"folderPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The relative path to the file name for the batch job identifier.\"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"fileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-file-batch-job-identifier-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: FileBatchJobIdentifier
---
