---
description: An object containing <code>SchemaName</code>, <code>SchemaArn</code>, <code>CreatedAt</code>, and<code>UpdatedAt</code>.
layout: schema
name: SchemaMappingSummary
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: schemaArn
  type: object
- description: ''
  name: schemaName
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-schema-mapping-summary-schema.json
slug: amazon-entity-resolution-schema-mapping-summary
source_filename: amazon-entity-resolution-schema-mapping-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-schema-mapping-summary-schema.json\",\n  \"title\": \"SchemaMappingSummary\",\n  \"description\": \"An object containing <code>SchemaName</code>, <code>SchemaArn</code>, <code>CreatedAt</code>, and<code>UpdatedAt</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the <code>SchemaMapping</code> was created.\"\n        }\n      ]\n    },\n    \"schemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaMappingArn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) that Entity Resolution generated for the <code>SchemaMapping</code>.\"\
  \n        }\n      ]\n    },\n    \"schemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the schema.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the <code>SchemaMapping</code> was last updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"schemaArn\",\n    \"schemaName\",\n    \"updatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-schema-mapping-summary-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: SchemaMappingSummary
---
