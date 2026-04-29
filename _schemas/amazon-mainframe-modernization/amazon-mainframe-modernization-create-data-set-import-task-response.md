---
description: CreateDataSetImportTaskResponse schema from AWS Mainframe Modernization API
layout: schema
name: CreateDataSetImportTaskResponse
properties_list:
- description: ''
  name: taskId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-data-set-import-task-response-schema.json
slug: amazon-mainframe-modernization-create-data-set-import-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-data-set-import-task-response-schema.json\",\n  \"title\": \"CreateDataSetImportTaskResponse\",\n  \"description\": \"CreateDataSetImportTaskResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The task identifier. This operation is asynchronous. Use this identifier with the <a>GetDataSetImportTask</a> operation to obtain the status of this task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"taskId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-data-set-import-task-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateDataSetImportTaskResponse
---
