---
description: GetRegistryInput schema from Amazon Glue API
layout: schema
name: GetRegistryInput
properties_list:
- description: ''
  name: RegistryId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-registry-input-schema.json
slug: glue-get-registry-input
source_filename: glue-get-registry-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-registry-input-schema.json\",\n  \"title\": \"GetRegistryInput\",\n  \"description\": \"GetRegistryInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryId\"\n        },\n        {\n          \"description\": \"This is a wrapper structure that may contain the registry name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RegistryId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-registry-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetRegistryInput
---
