---
description: BatchGetTriggersRequest schema from Amazon Glue API
layout: schema
name: BatchGetTriggersRequest
properties_list:
- description: ''
  name: TriggerNames
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-triggers-request-schema.json
slug: glue-batch-get-triggers-request
source_filename: glue-batch-get-triggers-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-triggers-request-schema.json\",\n  \"title\": \"BatchGetTriggersRequest\",\n  \"description\": \"BatchGetTriggersRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TriggerNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerNameList\"\n        },\n        {\n          \"description\": \"A list of trigger names, which may be the names returned from the <code>ListTriggers</code> operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TriggerNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-triggers-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetTriggersRequest
---
