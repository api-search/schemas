---
description: GetWorkflowRunPropertiesRequest schema from Amazon Glue API
layout: schema
name: GetWorkflowRunPropertiesRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-run-properties-request-schema.json
slug: glue-get-workflow-run-properties-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-properties-request-schema.json\",\n  \"title\": \"GetWorkflowRunPropertiesRequest\",\n  \"description\": \"GetWorkflowRunPropertiesRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the workflow which was run.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the workflow run whose run properties should be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-run-properties-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunPropertiesRequest
---
