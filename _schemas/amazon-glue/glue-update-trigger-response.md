---
description: UpdateTriggerResponse schema from Amazon Glue API
layout: schema
name: UpdateTriggerResponse
properties_list:
- description: ''
  name: Trigger
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-trigger-response-schema.json
slug: glue-update-trigger-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-trigger-response-schema.json\",\n  \"title\": \"UpdateTriggerResponse\",\n  \"description\": \"UpdateTriggerResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Trigger\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Trigger\"\n        },\n        {\n          \"description\": \"The resulting trigger definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-trigger-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateTriggerResponse
---
