---
description: GetTableVersionResponse schema from Amazon Glue API
layout: schema
name: GetTableVersionResponse
properties_list:
- description: ''
  name: TableVersion
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-table-version-response-schema.json
slug: glue-get-table-version-response
source_filename: glue-get-table-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-version-response-schema.json\",\n  \"title\": \"GetTableVersionResponse\",\n  \"description\": \"GetTableVersionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableVersion\"\n        },\n        {\n          \"description\": \"The requested table version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-version-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTableVersionResponse
---
