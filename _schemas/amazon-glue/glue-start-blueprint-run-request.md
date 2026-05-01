---
description: StartBlueprintRunRequest schema from Amazon Glue API
layout: schema
name: StartBlueprintRunRequest
properties_list:
- description: ''
  name: BlueprintName
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-blueprint-run-request-schema.json
slug: glue-start-blueprint-run-request
source_filename: glue-start-blueprint-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-blueprint-run-request-schema.json\",\n  \"title\": \"StartBlueprintRunRequest\",\n  \"description\": \"StartBlueprintRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlueprintName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n        {\n          \"description\": \"The name of the blueprint.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueprintParameters\"\n        },\n        {\n          \"description\": \"Specifies the parameters as a <code>BlueprintParameters</code> object.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationIAMRoleArn\"\
  \n        },\n        {\n          \"description\": \"Specifies the IAM role used to create the workflow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BlueprintName\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-blueprint-run-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartBlueprintRunRequest
---
