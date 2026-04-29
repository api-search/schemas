---
description: ListSchemaMappingsOutput schema from AWS EntityResolution
layout: schema
name: ListSchemaMappingsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: schemaList
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-list-schema-mappings-output-schema.json
slug: amazon-entity-resolution-list-schema-mappings-output
source_filename: amazon-entity-resolution-list-schema-mappings-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-list-schema-mappings-output-schema.json\",\n  \"title\": \"ListSchemaMappingsOutput\",\n  \"description\": \"ListSchemaMappingsOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token from the previous <code>ListDomains</code> API call.\"\n        }\n      ]\n    },\n    \"schemaList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaMappingList\"\n        },\n        {\n          \"description\": \"A list of <code>SchemaMappingSummary</code> objects, each of which contain the fields <code>SchemaName</code>, <code>SchemaArn</code>,\
  \ <code>CreatedAt</code>, <code>UpdatedAt</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-list-schema-mappings-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: ListSchemaMappingsOutput
---
