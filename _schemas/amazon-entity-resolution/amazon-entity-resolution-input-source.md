---
description: An object containing <code>InputSourceARN</code>, <code>SchemaName</code>, and <code>ApplyNormalization</code>.
layout: schema
name: InputSource
properties_list:
- description: ''
  name: applyNormalization
  type: object
- description: ''
  name: inputSourceARN
  type: object
- description: ''
  name: schemaName
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-input-source-schema.json
slug: amazon-entity-resolution-input-source
source_filename: amazon-entity-resolution-input-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-input-source-schema.json\",\n  \"title\": \"InputSource\",\n  \"description\": \"An object containing <code>InputSourceARN</code>, <code>SchemaName</code>, and <code>ApplyNormalization</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applyNormalization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Normalizes the attributes defined in the schema in the input data. For example, if an attribute has an <code>AttributeType</code> of <code>PHONE_NUMBER</code>, and the data in the input table is in a format of 1234567890, Entity Resolution will normalize this field in the output to (123)-456-7890.\"\n        }\n      ]\n    },\n    \"inputSourceARN\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/InputSourceInputSourceARNString\"\n        },\n        {\n          \"description\": \"An Glue table ARN for the input source table.\"\n        }\n      ]\n    },\n    \"schemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the schema to be retrieved.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputSourceARN\",\n    \"schemaName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-input-source-schema.json
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: InputSource
---
