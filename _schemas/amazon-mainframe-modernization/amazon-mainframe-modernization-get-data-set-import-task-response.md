---
description: GetDataSetImportTaskResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetDataSetImportTaskResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: taskId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-data-set-import-task-response-schema.json
slug: amazon-mainframe-modernization-get-data-set-import-task-response
source_filename: amazon-mainframe-modernization-get-data-set-import-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-data-set-import-task-response-schema.json\",\n  \"title\": \"GetDataSetImportTaskResponse\",\n  \"description\": \"GetDataSetImportTaskResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSetTaskLifecycle\"\n        },\n        {\n          \"description\": \"The status of the task.\"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSetImportSummary\"\n        },\n        {\n          \"description\": \"A summary of the status of the task.\"\n        }\n      ]\n    },\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The task identifier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"taskId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-data-set-import-task-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetDataSetImportTaskResponse
---
