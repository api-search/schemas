---
description: SearchTablesResponse schema from Amazon Glue API
layout: schema
name: SearchTablesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: TableList
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-search-tables-response-schema.json
slug: glue-search-tables-response
source_filename: glue-search-tables-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-search-tables-response-schema.json\",\n  \"title\": \"SearchTablesResponse\",\n  \"description\": \"SearchTablesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, present if the current list segment is not the last.\"\n        }\n      ]\n    },\n    \"TableList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableList\"\n        },\n        {\n          \"description\": \"A list of the requested <code>Table</code> objects. The <code>SearchTables</code> response returns only the tables that you have access to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-search-tables-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: SearchTablesResponse
---
