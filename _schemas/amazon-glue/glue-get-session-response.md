---
description: GetSessionResponse schema from Amazon Glue API
layout: schema
name: GetSessionResponse
properties_list:
- description: ''
  name: Session
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-session-response-schema.json
slug: glue-get-session-response
source_filename: glue-get-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-session-response-schema.json\",\n  \"title\": \"GetSessionResponse\",\n  \"description\": \"GetSessionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Session\"\n        },\n        {\n          \"description\": \"The session object is returned in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-session-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSessionResponse
---
