---
description: ''
layout: schema
name: ReplaceableAttribute
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: Replace
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-replaceable-attribute-schema.json
slug: amazon-simpledb-replaceable-attribute
source_filename: amazon-simpledb-replaceable-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-replaceable-attribute-schema.json\",\n  \"title\": \"ReplaceableAttribute\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the replaceable attribute.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the replaceable attribute.\"\n        }\n      ]\n    },\n    \"Replace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A flag specifying whether or not to replace\
  \ the attribute/value pair or to add a new attribute/value pair. The default setting is <code>false</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-replaceable-attribute-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: ReplaceableAttribute
---
