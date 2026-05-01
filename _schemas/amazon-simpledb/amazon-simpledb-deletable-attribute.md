---
description: ''
layout: schema
name: DeletableAttribute
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-deletable-attribute-schema.json
slug: amazon-simpledb-deletable-attribute
source_filename: amazon-simpledb-deletable-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-deletable-attribute-schema.json\",\n  \"title\": \"DeletableAttribute\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the attribute.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the attribute.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-deletable-attribute-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: DeletableAttribute
---
