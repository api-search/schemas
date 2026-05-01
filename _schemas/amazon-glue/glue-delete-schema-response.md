---
description: DeleteSchemaResponse schema from Amazon Glue API
layout: schema
name: DeleteSchemaResponse
properties_list:
- description: ''
  name: SchemaArn
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-schema-response-schema.json
slug: glue-delete-schema-response
source_filename: glue-delete-schema-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-response-schema.json\",\n  \"title\": \"DeleteSchemaResponse\",\n  \"description\": \"DeleteSchemaResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schema being deleted.\"\n        }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryNameString\"\n        },\n        {\n          \"description\": \"The name of the schema being deleted.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaStatus\"\n\
  \        },\n        {\n          \"description\": \"The status of the schema.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSchemaResponse
---
