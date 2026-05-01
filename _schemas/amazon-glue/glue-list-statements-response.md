---
description: ListStatementsResponse schema from Amazon Glue API
layout: schema
name: ListStatementsResponse
properties_list:
- description: ''
  name: Statements
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-statements-response-schema.json
slug: glue-list-statements-response
source_filename: glue-list-statements-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-statements-response-schema.json\",\n  \"title\": \"ListStatementsResponse\",\n  \"description\": \"ListStatementsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatementList\"\n        },\n        {\n          \"description\": \"Returns the list of statements.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationToken\"\n        },\n        {\n          \"description\": \"A continuation token, if not all statements have yet been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-statements-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListStatementsResponse
---
