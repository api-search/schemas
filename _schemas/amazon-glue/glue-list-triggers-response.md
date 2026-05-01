---
description: ListTriggersResponse schema from Amazon Glue API
layout: schema
name: ListTriggersResponse
properties_list:
- description: ''
  name: TriggerNames
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-triggers-response-schema.json
slug: glue-list-triggers-response
source_filename: glue-list-triggers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-triggers-response-schema.json\",\n  \"title\": \"ListTriggersResponse\",\n  \"description\": \"ListTriggersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TriggerNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerNameList\"\n        },\n        {\n          \"description\": \"The names of all triggers in the account, or the triggers with the specified tags.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list does not contain the last metric available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-triggers-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListTriggersResponse
---
