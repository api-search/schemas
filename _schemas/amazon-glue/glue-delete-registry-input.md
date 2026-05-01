---
description: DeleteRegistryInput schema from Amazon Glue API
layout: schema
name: DeleteRegistryInput
properties_list:
- description: ''
  name: RegistryId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-registry-input-schema.json
slug: glue-delete-registry-input
source_filename: glue-delete-registry-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-registry-input-schema.json\",\n  \"title\": \"DeleteRegistryInput\",\n  \"description\": \"DeleteRegistryInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryId\"\n        },\n        {\n          \"description\": \"This is a wrapper structure that may contain the registry name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RegistryId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-registry-input-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteRegistryInput
---
