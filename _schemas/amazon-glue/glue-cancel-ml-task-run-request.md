---
description: CancelMLTaskRunRequest schema from Amazon Glue API
layout: schema
name: CancelMLTaskRunRequest
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: TaskRunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-cancel-ml-task-run-request-schema.json
slug: glue-cancel-ml-task-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-cancel-ml-task-run-request-schema.json\",\n  \"title\": \"CancelMLTaskRunRequest\",\n  \"description\": \"CancelMLTaskRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the machine learning transform.\"\n        }\n      ]\n    },\n    \"TaskRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"A unique identifier for the task run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransformId\",\n    \"TaskRunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-cancel-ml-task-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CancelMLTaskRunRequest
---
