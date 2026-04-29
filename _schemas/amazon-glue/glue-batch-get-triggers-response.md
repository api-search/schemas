---
description: BatchGetTriggersResponse schema from Amazon Glue API
layout: schema
name: BatchGetTriggersResponse
properties_list:
- description: ''
  name: Triggers
  type: object
- description: ''
  name: TriggersNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-triggers-response-schema.json
slug: glue-batch-get-triggers-response
source_filename: glue-batch-get-triggers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-triggers-response-schema.json\",\n  \"title\": \"BatchGetTriggersResponse\",\n  \"description\": \"BatchGetTriggersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Triggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerList\"\n        },\n        {\n          \"description\": \"A list of trigger definitions.\"\n        }\n      ]\n    },\n    \"TriggersNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerNameList\"\n        },\n        {\n          \"description\": \"A list of names of triggers not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-triggers-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetTriggersResponse
---
