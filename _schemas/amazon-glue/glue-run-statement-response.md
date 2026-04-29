---
description: RunStatementResponse schema from Amazon Glue API
layout: schema
name: RunStatementResponse
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-run-statement-response-schema.json
slug: glue-run-statement-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-run-statement-response-schema.json\",\n  \"title\": \"RunStatementResponse\",\n  \"description\": \"RunStatementResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"description\": \"Returns the Id of the statement that was run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-run-statement-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: RunStatementResponse
---
