---
description: CreateSchemaMappingInput schema from AWS EntityResolution
layout: schema
name: CreateSchemaMappingInput
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: mappedInputFields
  type: object
- description: ''
  name: schemaName
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-create-schema-mapping-input-schema.json
slug: amazon-entity-resolution-create-schema-mapping-input
source_filename: amazon-entity-resolution-create-schema-mapping-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-create-schema-mapping-input-schema.json\",\n  \"title\": \"CreateSchemaMappingInput\",\n  \"description\": \"CreateSchemaMappingInput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the schema.\"\n        }\n      ]\n    },\n    \"mappedInputFields\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaInputAttributes\"\n        },\n        {\n          \"description\": \"A list of <code>MappedInputFields</code>. Each <code>MappedInputField</code> corresponds to a column the source data table, and contains column name plus additional\
  \ information that Entity Resolution uses for matching.\"\n        }\n      ]\n    },\n    \"schemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the schema. There cannot be multiple <code>SchemaMappings</code> with the same name.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags used to organize, track, or control access for this resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"schemaName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-create-schema-mapping-input-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: CreateSchemaMappingInput
---
