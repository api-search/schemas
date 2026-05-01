---
description: GetRegistryResponse schema from Amazon Glue API
layout: schema
name: GetRegistryResponse
properties_list:
- description: ''
  name: RegistryName
  type: object
- description: ''
  name: RegistryArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: UpdatedTime
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-registry-response-schema.json
slug: glue-get-registry-response
source_filename: glue-get-registry-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-registry-response-schema.json\",\n  \"title\": \"GetRegistryResponse\",\n  \"description\": \"GetRegistryResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the registry.\"\n        }\n      ]\n    },\n    \"RegistryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the registry.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n\
  \        {\n          \"description\": \"A description of the registry.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryStatus\"\n        },\n        {\n          \"description\": \"The status of the registry.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the registry was created.\"\n        }\n      ]\n    },\n    \"UpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the registry was updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-registry-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetRegistryResponse
---
