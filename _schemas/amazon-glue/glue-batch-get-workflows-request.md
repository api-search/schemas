---
description: BatchGetWorkflowsRequest schema from Amazon Glue API
layout: schema
name: BatchGetWorkflowsRequest
properties_list:
- description: ''
  name: Names
  type: object
- description: ''
  name: IncludeGraph
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-workflows-request-schema.json
slug: glue-batch-get-workflows-request
source_filename: glue-batch-get-workflows-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-workflows-request-schema.json\",\n  \"title\": \"BatchGetWorkflowsRequest\",\n  \"description\": \"BatchGetWorkflowsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowNames\"\n        },\n        {\n          \"description\": \"A list of workflow names, which may be the names returned from the <code>ListWorkflows</code> operation.\"\n        }\n      ]\n    },\n    \"IncludeGraph\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether to include a graph when returning the workflow resource metadata.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Names\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-workflows-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetWorkflowsRequest
---
