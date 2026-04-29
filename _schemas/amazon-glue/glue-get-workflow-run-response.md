---
description: GetWorkflowRunResponse schema from Amazon Glue API
layout: schema
name: GetWorkflowRunResponse
properties_list:
- description: ''
  name: Run
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-run-response-schema.json
slug: glue-get-workflow-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-response-schema.json\",\n  \"title\": \"GetWorkflowRunResponse\",\n  \"description\": \"GetWorkflowRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Run\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRun\"\n        },\n        {\n          \"description\": \"The requested workflow run metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunResponse
---
