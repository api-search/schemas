---
description: GetSchemaVersionsDiffResponse schema from Amazon Glue API
layout: schema
name: GetSchemaVersionsDiffResponse
properties_list:
- description: ''
  name: Diff
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-schema-versions-diff-response-schema.json
slug: glue-get-schema-versions-diff-response
source_filename: glue-get-schema-versions-diff-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-versions-diff-response-schema.json\",\n  \"title\": \"GetSchemaVersionsDiffResponse\",\n  \"description\": \"GetSchemaVersionsDiffResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Diff\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDefinitionDiff\"\n        },\n        {\n          \"description\": \"The difference between schemas as a string in JsonPatch format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-schema-versions-diff-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSchemaVersionsDiffResponse
---
