---
description: UpdateRegistryResponse schema from Amazon Glue API
layout: schema
name: UpdateRegistryResponse
properties_list:
- description: ''
  name: RegistryName
  type: object
- description: ''
  name: RegistryArn
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-registry-response-schema.json
slug: glue-update-registry-response
source_filename: glue-update-registry-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-registry-response-schema.json\",\n  \"title\": \"UpdateRegistryResponse\",\n  \"description\": \"UpdateRegistryResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the updated registry.\"\n        }\n      ]\n    },\n    \"RegistryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource name (ARN) of the updated registry.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-registry-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateRegistryResponse
---
