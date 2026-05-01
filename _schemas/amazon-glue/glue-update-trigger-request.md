---
description: UpdateTriggerRequest schema from Amazon Glue API
layout: schema
name: UpdateTriggerRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: TriggerUpdate
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-trigger-request-schema.json
slug: glue-update-trigger-request
source_filename: glue-update-trigger-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-trigger-request-schema.json\",\n  \"title\": \"UpdateTriggerRequest\",\n  \"description\": \"UpdateTriggerRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the trigger to update.\"\n        }\n      ]\n    },\n    \"TriggerUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerUpdate\"\n        },\n        {\n          \"description\": \"The new values with which to update the trigger.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"TriggerUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-trigger-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateTriggerRequest
---
