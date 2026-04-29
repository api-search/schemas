---
description: StartWorkflowRunRequest schema from Amazon Glue API
layout: schema
name: StartWorkflowRunRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunProperties
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-workflow-run-request-schema.json
slug: glue-start-workflow-run-request
source_filename: glue-start-workflow-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-workflow-run-request-schema.json\",\n  \"title\": \"StartWorkflowRunRequest\",\n  \"description\": \"StartWorkflowRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the workflow to start.\"\n        }\n      ]\n    },\n    \"RunProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunProperties\"\n        },\n        {\n          \"description\": \"The workflow run properties for the new workflow run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-workflow-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartWorkflowRunRequest
---
