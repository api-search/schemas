---
description: DeleteRegistryResponse schema from Amazon Glue API
layout: schema
name: DeleteRegistryResponse
properties_list:
- description: ''
  name: RegistryName
  type: object
- description: ''
  name: RegistryArn
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-registry-response-schema.json
slug: glue-delete-registry-response
source_filename: glue-delete-registry-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-registry-response-schema.json\",\n  \"title\": \"DeleteRegistryResponse\",\n  \"description\": \"DeleteRegistryResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the registry being deleted.\"\n        }\n      ]\n    },\n    \"RegistryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the registry being deleted.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryStatus\"\
  \n        },\n        {\n          \"description\": \"The status of the registry. A successful operation will return the <code>Deleting</code> status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-registry-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteRegistryResponse
---
