---
description: GetTablesResponse schema from Amazon Glue API
layout: schema
name: GetTablesResponse
properties_list:
- description: ''
  name: TableList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-tables-response-schema.json
slug: glue-get-tables-response
source_filename: glue-get-tables-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-tables-response-schema.json\",\n  \"title\": \"GetTablesResponse\",\n  \"description\": \"GetTablesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableList\"\n        },\n        {\n          \"description\": \"A list of the requested <code>Table</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, present if the current list segment is not the last.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-tables-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTablesResponse
---
