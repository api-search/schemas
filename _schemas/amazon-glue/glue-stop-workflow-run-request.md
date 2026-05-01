---
description: StopWorkflowRunRequest schema from Amazon Glue API
layout: schema
name: StopWorkflowRunRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-stop-workflow-run-request-schema.json
slug: glue-stop-workflow-run-request
source_filename: glue-stop-workflow-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-workflow-run-request-schema.json\",\n  \"title\": \"StopWorkflowRunRequest\",\n  \"description\": \"StopWorkflowRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the workflow to stop.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the workflow run to stop.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-workflow-run-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StopWorkflowRunRequest
---
