---
description: BatchGetWorkflowsResponse schema from Amazon Glue API
layout: schema
name: BatchGetWorkflowsResponse
properties_list:
- description: ''
  name: Workflows
  type: object
- description: ''
  name: MissingWorkflows
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-workflows-response-schema.json
slug: glue-batch-get-workflows-response
source_filename: glue-batch-get-workflows-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-workflows-response-schema.json\",\n  \"title\": \"BatchGetWorkflowsResponse\",\n  \"description\": \"BatchGetWorkflowsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Workflows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Workflows\"\n        },\n        {\n          \"description\": \"A list of workflow resource metadata.\"\n        }\n      ]\n    },\n    \"MissingWorkflows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowNames\"\n        },\n        {\n          \"description\": \"A list of names of workflows not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-workflows-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetWorkflowsResponse
---
