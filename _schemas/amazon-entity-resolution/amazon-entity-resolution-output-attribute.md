---
description: A list of <code>OutputAttribute</code> objects, each of which have the fields Name and Hashed. Each of these objects selects a column to be included in the output table, and whether the values of the column should be hashed.
layout: schema
name: OutputAttribute
properties_list:
- description: ''
  name: hashed
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-output-attribute-schema.json
slug: amazon-entity-resolution-output-attribute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-output-attribute-schema.json\",\n  \"title\": \"OutputAttribute\",\n  \"description\": \"A list of <code>OutputAttribute</code> objects, each of which have the fields Name and Hashed. Each of these objects selects a column to be included in the output table, and whether the values of the column should be hashed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hashed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Enables the ability to hash the column values in the output.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeName\"\n        },\n        {\n          \"description\": \"A name\
  \ of a column to be written to the output. This must be an <code>InputField</code> name in the schema mapping.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-output-attribute-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: OutputAttribute
---
