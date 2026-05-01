---
description: DeleteSessionResponse schema from Amazon Glue API
layout: schema
name: DeleteSessionResponse
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-session-response-schema.json
slug: glue-delete-session-response
source_filename: glue-delete-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-session-response-schema.json\",\n  \"title\": \"DeleteSessionResponse\",\n  \"description\": \"DeleteSessionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Returns the ID of the deleted session.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-session-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSessionResponse
---
