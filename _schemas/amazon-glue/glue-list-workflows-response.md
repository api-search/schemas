---
description: ListWorkflowsResponse schema from Amazon Glue API
layout: schema
name: ListWorkflowsResponse
properties_list:
- description: ''
  name: Workflows
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-workflows-response-schema.json
slug: glue-list-workflows-response
source_filename: glue-list-workflows-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-workflows-response-schema.json\",\n  \"title\": \"ListWorkflowsResponse\",\n  \"description\": \"ListWorkflowsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Workflows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowNames\"\n        },\n        {\n          \"description\": \"List of names of workflows in the account.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all workflow names have been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-workflows-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListWorkflowsResponse
---
