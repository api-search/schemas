---
description: GetMappingResponse schema from Amazon Glue API
layout: schema
name: GetMappingResponse
properties_list:
- description: ''
  name: Mapping
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-mapping-response-schema.json
slug: glue-get-mapping-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-mapping-response-schema.json\",\n  \"title\": \"GetMappingResponse\",\n  \"description\": \"GetMappingResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MappingList\"\n        },\n        {\n          \"description\": \"A list of mappings to the specified targets.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Mapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-mapping-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMappingResponse
---
