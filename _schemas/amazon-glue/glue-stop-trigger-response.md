---
description: StopTriggerResponse schema from Amazon Glue API
layout: schema
name: StopTriggerResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-stop-trigger-response-schema.json
slug: glue-stop-trigger-response
source_filename: glue-stop-trigger-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-trigger-response-schema.json\",\n  \"title\": \"StopTriggerResponse\",\n  \"description\": \"StopTriggerResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the trigger that was stopped.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-trigger-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StopTriggerResponse
---
