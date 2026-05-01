---
description: GetWorkflowRequest schema from Amazon Glue API
layout: schema
name: GetWorkflowRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: IncludeGraph
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-request-schema.json
slug: glue-get-workflow-request
source_filename: glue-get-workflow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-request-schema.json\",\n  \"title\": \"GetWorkflowRequest\",\n  \"description\": \"GetWorkflowRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the workflow to retrieve.\"\n        }\n      ]\n    },\n    \"IncludeGraph\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether to include a graph when returning the workflow resource metadata.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRequest
---
