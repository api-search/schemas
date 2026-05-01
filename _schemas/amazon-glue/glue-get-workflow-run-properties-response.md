---
description: GetWorkflowRunPropertiesResponse schema from Amazon Glue API
layout: schema
name: GetWorkflowRunPropertiesResponse
properties_list:
- description: ''
  name: RunProperties
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-run-properties-response-schema.json
slug: glue-get-workflow-run-properties-response
source_filename: glue-get-workflow-run-properties-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-properties-response-schema.json\",\n  \"title\": \"GetWorkflowRunPropertiesResponse\",\n  \"description\": \"GetWorkflowRunPropertiesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunProperties\"\n        },\n        {\n          \"description\": \"The workflow run properties which were set during the specified run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-properties-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunPropertiesResponse
---
