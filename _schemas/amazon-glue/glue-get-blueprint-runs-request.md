---
description: GetBlueprintRunsRequest schema from Amazon Glue API
layout: schema
name: GetBlueprintRunsRequest
properties_list:
- description: ''
  name: BlueprintName
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-blueprint-runs-request-schema.json
slug: glue-get-blueprint-runs-request
source_filename: glue-get-blueprint-runs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-runs-request-schema.json\",\n  \"title\": \"GetBlueprintRunsRequest\",\n  \"description\": \"GetBlueprintRunsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlueprintName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the blueprint.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation request.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n    \
  \    {\n          \"description\": \"The maximum size of a list to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BlueprintName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-blueprint-runs-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetBlueprintRunsRequest
---
