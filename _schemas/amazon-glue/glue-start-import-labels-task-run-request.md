---
description: StartImportLabelsTaskRunRequest schema from Amazon Glue API
layout: schema
name: StartImportLabelsTaskRunRequest
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: InputS3Path
  type: object
- description: ''
  name: ReplaceAllLabels
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-import-labels-task-run-request-schema.json
slug: glue-start-import-labels-task-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-import-labels-task-run-request-schema.json\",\n  \"title\": \"StartImportLabelsTaskRunRequest\",\n  \"description\": \"StartImportLabelsTaskRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the machine learning transform.\"\n        }\n      ]\n    },\n    \"InputS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UriString\"\n        },\n        {\n          \"description\": \"The Amazon Simple Storage Service (Amazon S3) path from where you import the labels.\"\n        }\n      ]\n    },\n    \"ReplaceAllLabels\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/ReplaceBoolean\"\n        },\n        {\n          \"description\": \"Indicates whether to overwrite your existing labels.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransformId\",\n    \"InputS3Path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-import-labels-task-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartImportLabelsTaskRunRequest
---
