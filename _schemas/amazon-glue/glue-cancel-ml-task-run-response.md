---
description: CancelMLTaskRunResponse schema from Amazon Glue API
layout: schema
name: CancelMLTaskRunResponse
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: TaskRunId
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-cancel-ml-task-run-response-schema.json
slug: glue-cancel-ml-task-run-response
source_filename: glue-cancel-ml-task-run-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-cancel-ml-task-run-response-schema.json\",\n  \"title\": \"CancelMLTaskRunResponse\",\n  \"description\": \"CancelMLTaskRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the machine learning transform.\"\n        }\n      ]\n    },\n    \"TaskRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier for the task run.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatusType\"\n     \
  \   },\n        {\n          \"description\": \"The status for this run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-cancel-ml-task-run-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CancelMLTaskRunResponse
---
