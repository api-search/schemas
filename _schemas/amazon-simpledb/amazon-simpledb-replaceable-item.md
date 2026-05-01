---
description: ''
layout: schema
name: ReplaceableItem
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-replaceable-item-schema.json
slug: amazon-simpledb-replaceable-item
source_filename: amazon-simpledb-replaceable-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-replaceable-item-schema.json\",\n  \"title\": \"ReplaceableItem\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ItemName\"\n          },\n          \"description\": \"The name of the replaceable item.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplaceableAttributeList\"\n        },\n        {\n          \"description\": \"The list of attributes for a replaceable item.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Attributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-replaceable-item-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: ReplaceableItem
---
