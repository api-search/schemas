---
description: GetWorkflowRunRequest schema from Amazon Glue API
layout: schema
name: GetWorkflowRunRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunId
  type: object
- description: ''
  name: IncludeGraph
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-run-request-schema.json
slug: glue-get-workflow-run-request
source_filename: glue-get-workflow-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-request-schema.json\",\n  \"title\": \"GetWorkflowRunRequest\",\n  \"description\": \"GetWorkflowRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the workflow being run.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the workflow run.\"\n        }\n      ]\n    },\n    \"IncludeGraph\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies\
  \ whether to include the workflow graph in response or not.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunRequest
---
