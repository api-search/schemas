---
description: StartMLLabelingSetGenerationTaskRunResponse schema from Amazon Glue API
layout: schema
name: StartMLLabelingSetGenerationTaskRunResponse
properties_list:
- description: ''
  name: TaskRunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-ml-labeling-set-generation-task-run-response-schema.json
slug: glue-start-ml-labeling-set-generation-task-run-response
source_filename: glue-start-ml-labeling-set-generation-task-run-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-ml-labeling-set-generation-task-run-response-schema.json\",\n  \"title\": \"StartMLLabelingSetGenerationTaskRunResponse\",\n  \"description\": \"StartMLLabelingSetGenerationTaskRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run identifier that is associated with this task run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-ml-labeling-set-generation-task-run-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartMLLabelingSetGenerationTaskRunResponse
---
