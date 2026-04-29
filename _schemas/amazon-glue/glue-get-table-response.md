---
description: GetTableResponse schema from Amazon Glue API
layout: schema
name: GetTableResponse
properties_list:
- description: ''
  name: Table
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-table-response-schema.json
slug: glue-get-table-response
source_filename: glue-get-table-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-response-schema.json\",\n  \"title\": \"GetTableResponse\",\n  \"description\": \"GetTableResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Table\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Table\"\n        },\n        {\n          \"description\": \"The <code>Table</code> object that defines the specified table.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTableResponse
---
