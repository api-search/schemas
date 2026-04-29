---
description: GetTriggersResponse schema from Amazon Glue API
layout: schema
name: GetTriggersResponse
properties_list:
- description: ''
  name: Triggers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-triggers-response-schema.json
slug: glue-get-triggers-response
source_filename: glue-get-triggers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-triggers-response-schema.json\",\n  \"title\": \"GetTriggersResponse\",\n  \"description\": \"GetTriggersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Triggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerList\"\n        },\n        {\n          \"description\": \"A list of triggers for the specified job.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all the requested triggers have yet been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-triggers-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTriggersResponse
---
