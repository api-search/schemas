---
description: DeleteSchemaInput schema from Amazon Glue API
layout: schema
name: DeleteSchemaInput
properties_list:
- description: ''
  name: SchemaId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-schema-input-schema.json
slug: glue-delete-schema-input
source_filename: glue-delete-schema-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-input-schema.json\",\n  \"title\": \"DeleteSchemaInput\",\n  \"description\": \"DeleteSchemaInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"This is a wrapper structure that may contain the schema name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SchemaId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-schema-input-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteSchemaInput
---
