---
description: GetSchemaMappingOutput schema from AWS EntityResolution
layout: schema
name: GetSchemaMappingOutput
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: mappedInputFields
  type: object
- description: ''
  name: schemaArn
  type: object
- description: ''
  name: schemaName
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-get-schema-mapping-output-schema.json
slug: amazon-entity-resolution-get-schema-mapping-output
source_filename: amazon-entity-resolution-get-schema-mapping-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-schema-mapping-output-schema.json\",\n  \"title\": \"GetSchemaMappingOutput\",\n  \"description\": \"GetSchemaMappingOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the <code>SchemaMapping</code> was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the schema.\"\n        }\n      ]\n    },\n    \"mappedInputFields\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaInputAttributes\"\
  \n        },\n        {\n          \"description\": \"A list of <code>MappedInputFields</code>. Each <code>MappedInputField</code> corresponds to a column the source data table, and contains column name plus additional information Venice uses for matching.\"\n        }\n      ]\n    },\n    \"schemaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaMappingArn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) that Entity Resolution generated for the SchemaMapping.\"\n        }\n      ]\n    },\n    \"schemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the schema.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags used to organize, track, or control access for\
  \ this resource.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the <code>SchemaMapping</code> was last updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"mappedInputFields\",\n    \"schemaArn\",\n    \"schemaName\",\n    \"updatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-schema-mapping-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: GetSchemaMappingOutput
---
