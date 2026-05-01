---
description: GetDatabaseResponse schema from Amazon Glue API
layout: schema
name: GetDatabaseResponse
properties_list:
- description: ''
  name: Database
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-database-response-schema.json
slug: glue-get-database-response
source_filename: glue-get-database-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-database-response-schema.json\",\n  \"title\": \"GetDatabaseResponse\",\n  \"description\": \"GetDatabaseResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Database\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Database\"\n        },\n        {\n          \"description\": \"The definition of the specified database in the Data Catalog.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-database-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDatabaseResponse
---
