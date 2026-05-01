---
description: GetStatementResponse schema from Amazon Glue API
layout: schema
name: GetStatementResponse
properties_list:
- description: ''
  name: Statement
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-statement-response-schema.json
slug: glue-get-statement-response
source_filename: glue-get-statement-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-statement-response-schema.json\",\n  \"title\": \"GetStatementResponse\",\n  \"description\": \"GetStatementResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Statement\"\n        },\n        {\n          \"description\": \"Returns the statement.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-statement-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetStatementResponse
---
