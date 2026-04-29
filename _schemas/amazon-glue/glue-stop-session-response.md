---
description: StopSessionResponse schema from Amazon Glue API
layout: schema
name: StopSessionResponse
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-stop-session-response-schema.json
slug: glue-stop-session-response
source_filename: glue-stop-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-session-response-schema.json\",\n  \"title\": \"StopSessionResponse\",\n  \"description\": \"StopSessionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Returns the Id of the stopped session.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-session-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StopSessionResponse
---
