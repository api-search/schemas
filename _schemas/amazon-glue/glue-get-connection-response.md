---
description: GetConnectionResponse schema from Amazon Glue API
layout: schema
name: GetConnectionResponse
properties_list:
- description: ''
  name: Connection
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-connection-response-schema.json
slug: glue-get-connection-response
source_filename: glue-get-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connection-response-schema.json\",\n  \"title\": \"GetConnectionResponse\",\n  \"description\": \"GetConnectionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Connection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Connection\"\n        },\n        {\n          \"description\": \"The requested connection definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connection-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetConnectionResponse
---
