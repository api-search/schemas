---
description: CheckSchemaVersionValidityInput schema from Amazon Glue API
layout: schema
name: CheckSchemaVersionValidityInput
properties_list:
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: SchemaDefinition
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-check-schema-version-validity-input-schema.json
slug: glue-check-schema-version-validity-input
source_filename: glue-check-schema-version-validity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-check-schema-version-validity-input-schema.json\",\n  \"title\": \"CheckSchemaVersionValidityInput\",\n  \"description\": \"CheckSchemaVersionValidityInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataFormat\"\n        },\n        {\n          \"description\": \"The data format of the schema definition. Currently <code>AVRO</code>, <code>JSON</code> and <code>PROTOBUF</code> are supported.\"\n        }\n      ]\n    },\n    \"SchemaDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaDefinitionString\"\n        },\n        {\n          \"description\": \"The definition of the schema that has to be validated.\"\n        }\n   \
  \   ]\n    }\n  },\n  \"required\": [\n    \"DataFormat\",\n    \"SchemaDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-check-schema-version-validity-input-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CheckSchemaVersionValidityInput
---
