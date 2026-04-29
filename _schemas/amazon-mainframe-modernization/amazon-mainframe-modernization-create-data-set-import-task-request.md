---
description: CreateDataSetImportTaskRequest schema from AWS Mainframe Modernization API
layout: schema
name: CreateDataSetImportTaskRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: importConfig
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-data-set-import-task-request-schema.json
slug: amazon-mainframe-modernization-create-data-set-import-task-request
source_filename: amazon-mainframe-modernization-create-data-set-import-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-data-set-import-task-request-schema.json\",\n  \"title\": \"CreateDataSetImportTaskRequest\",\n  \"description\": \"CreateDataSetImportTaskRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Unique, case-sensitive identifier you provide to ensure the idempotency of the request to create a data set import. The service generates the clientToken when the API call is triggered. The token expires after one hour, so if you retry the API within this timeframe with the same clientToken, you will get the same response. The service also handles deleting\
  \ the clientToken after it expires. \"\n        }\n      ]\n    },\n    \"importConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSetImportConfig\"\n        },\n        {\n          \"description\": \"The data set import task configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"importConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-data-set-import-task-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateDataSetImportTaskRequest
---
