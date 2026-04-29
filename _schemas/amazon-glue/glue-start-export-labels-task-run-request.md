---
description: StartExportLabelsTaskRunRequest schema from Amazon Glue API
layout: schema
name: StartExportLabelsTaskRunRequest
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: OutputS3Path
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-export-labels-task-run-request-schema.json
slug: glue-start-export-labels-task-run-request
source_filename: glue-start-export-labels-task-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-export-labels-task-run-request-schema.json\",\n  \"title\": \"StartExportLabelsTaskRunRequest\",\n  \"description\": \"StartExportLabelsTaskRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the machine learning transform.\"\n        }\n      ]\n    },\n    \"OutputS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UriString\"\n        },\n        {\n          \"description\": \"The Amazon S3 path where you export the labels.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransformId\",\n    \"OutputS3Path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-export-labels-task-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartExportLabelsTaskRunRequest
---
